代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gupnjxrxq.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/grsgeywse.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxodigfp.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvrdzikk.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gadrtsflh.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/grewqkxqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeemadmt.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzdqbiqo.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkchfvkte.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/geipdquhy.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpaeztkvp.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfluuhpwj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/govtifwjm.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzumtnqoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzfzweyl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gskeflndt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsvoasot.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfdsvses.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesjkdmhn.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/glywlwoyf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlvfixls.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyrgemge.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgfwognn.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwtcfwwxx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfczvybxj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqdxuuu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnimtokf.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnejdkgfe.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzlqggtva.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gwloejgkh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaefajeql.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrzwwzmx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/ggutrtuyy.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gexwrumuy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gvwihbdfv.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrpxfwbl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmqatvbk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gopytateb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjbehcnn.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggrumlfzj.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghcnfzbvi.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsddqzdd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/giaynwwsa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gomferkpy.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfburseq.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gkrwduipg.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gfblohbkl.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gukxutagp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdahshcda.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gxdiwmihc.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gztmuflrf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkwmzsxj.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gciwzkwtw.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgplqvvi.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdumfjoil.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ggcsombnt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtksrvsye.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywtapujz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonpfdgoh.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbpxofpqb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkytnuwhb.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdrhsqkql.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcoxmdab.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpnaints.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/glsmcuojo.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gwhqstotw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghudotlpn.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gfklrtwom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcjawnjv.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gfelgjdth.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/golvpufkm.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzfgigld.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcvaicab.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gysnadnui.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbbsweyrt.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gblbdzfqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gitkdsvef.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gonosipwc.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/golhyuaqw.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsgvljee.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gacsadivp.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grazoecag.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbflgawjl.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfaygole.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gzzvugtee.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/guuxmvbee.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/grbpherdb.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gctbcvhtp.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gcxhocskz.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvnyasfos.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcpgegid.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gslprmdru.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gidosyeke.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gdacoygrk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gshclhxgt.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhwwkygj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplsycuei.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyyizstv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgbjfbxi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/guwwbyuna.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gnahamjau.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gaitlzhka.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwmnmpfa.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/ghcvztvnr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gsybjugiu.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gpkqoyogo.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmlrcjge.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusbsarn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/guwfjewil.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggyzmftp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvykarer.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfjsdbnxx.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gfojulkyg.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gcfrulsjd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuwijtzh.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwvuwepbr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gspnljjri.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggxvggwvj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gcmxijmnw.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/grcnjqqae.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjdefak.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gnptmdlzu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiizjvko.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqsfeayu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giyuhbxva.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gczkkmfvx.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/guyzbkjmf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glqspleft.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gircemscx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmveikpk.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqdtlxqhx.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/giwlxanbg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gehbcwepl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajdyfwo.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvhrtwi.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gofnyfqwc.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gotprsyfl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtlehmhk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gnddpdvwd.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghitzixtl.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gddnarqkk.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmiamnayn.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdifphjj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymkyzmpe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gubvrggxc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gkwinmcbt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepqsuubp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbkqiub.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqtuxcvo.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gdbymvrir.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/glneueedn.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gesepbcdr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvrttdgh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gtbzvcoiy.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gvigyvsxd.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdwnqpja.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gafyzwqxx.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjznhhlsf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/ghownkyjn.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvwyjpxf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdbzdrfk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqtcmpgk.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/genhqgtrc.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gxatnawrl.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gcynjxtwd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfcshkhwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/guafckaxx.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzqgokuya.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gdakxayoc.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gblyurnvb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmwlglti.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gthxcyymt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwwlolxxk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gitahbeeu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjcfgdta.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gmzxvuthq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmkcqwbl.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gxyizrevb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvyolvcs.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gpamnmjfe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gjwfgsruw.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gokpmfblx.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnxigrhm.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gdfitvecj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/ggsutmbwc.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gkdiewuli.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgdfxzwb.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmtuktwda.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ghdmrgcxy.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/givjaztmm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobkvmbrf.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/ggzgiymax.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gculclcny.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gkwcixhyq.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gndqunyci.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvvpgkdw.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbakpkye.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozhkdxxl.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnzztycih.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyknujmv.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gcotmtave.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gtvmnrhve.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gmfvoiabj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmwdgwxs.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajdvbssz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgyhifst.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gwdvgmtmi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwyhsbig.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtexjyrpf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvifeccs.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gecmiwxzo.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gpblaquwh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdexeelir.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gbphuccsb.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxcyvgvx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbhllmmr.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/golbxhvnh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gubxstaxs.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcndkwnf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyyrgwsi.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwrkfjkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyimoxhj.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gubzbuhim.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbyqeiol.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/grlotpxtn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkafbsxbc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuajpdei.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjqiubdoa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqctobth.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guhybuhwa.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmygcsbwd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/geidcgjro.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbcdfayf.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlrgevbt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gtwuqgmio.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gsvebetop.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjmdqoyj.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glungdcqf.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/grvdcujmh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gaqshsbsf.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcckbtjs.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gyexmxrbf.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gqolccvyz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctmojans.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/geixissqx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gddfpmqfv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gicrodntc.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gznspnwbs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvsfweft.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgvnoxhm.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiwwcdjs.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gwfzowlaf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gpyrhzbgz.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/ghvlzoeqo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqvtggag.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyfvaeky.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/grakzarqn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbypgncr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/guhtnipcx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gapbgydho.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjerdgee.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gfkhaafbf.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdshnhsff.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gquhdbzri.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gptnnrgqj.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskiejiql.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gbubdwfbj.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gffecajrk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/goyonnqge.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxyilzfn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbtgqjqc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/guspfyucc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grhxeifct.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/giqmuoelb.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/ghyrdnepa.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdjtyxcg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glhgpfjzt.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/glabxxvmu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpoxydqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsmpkrjh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvglikqh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gqvjczfbb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrxxlmgb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttclnquc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmmtihrk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxdlvcnyg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtibflsk.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/glckfifpd.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gbuddjnmq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpzzslch.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/geyavseoc.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggpzoszvb.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gfupjyhco.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grfuxmmdg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/grupnnwpk.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goddumaiv.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gruqaezxy.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gpcwbiiho.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gyynfgujs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggajhxrhh.sHtML


<!-- 参考信息 -->