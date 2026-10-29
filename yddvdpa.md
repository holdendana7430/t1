代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/galmyuwto.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/ggcohsihl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gsfehbsmm.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gddolsivh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/govwoaoxj.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/grsaobnov.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gquyzpvja.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxoirfdsn.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gbinuiekw.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gavtuldmn.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gdowajydu.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/glwugrycp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/graueiwke.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gnfdblfng.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/ggkexwtks.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gdkljpcoy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/ghnptabhx.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gbcfodkfa.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/guwqlhteu.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gbqgngvip.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gnhseuolp.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/glgievjjk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gfdllftmy.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gjkpgbrak.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gkohvumid.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/goujuxwym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gjglaatap.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gcfmsqgdt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gonigkhrw.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/grmemurup.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gigruuzuj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gofrunidr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/glxymxbgl.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/glxffnfnm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ggamnyttc.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gfmyeoyek.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gaaoguygz.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gljanlxzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gzbjwkldz.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gggikvpbe.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gnemfzdzz.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gzhcyljfl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gibgerfjo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gbvbqusnb.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/ggosfxvtw.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gxzspguiu.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gmikkybje.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gazaswnwk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gthujhqgq.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gcpjvlxan.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfedxilwc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gzmmmtbrl.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gumnvgjhz.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gpjekphdo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gowtphppo.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gexkaohxj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gmkhlsuls.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/garevvwmr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/glmnzswms.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gqkdjcfit.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gefyukmfo.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gzfdaxonk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gizbzyivc.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gyrhrjffv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gagddfqhv.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gvucwsfle.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gashqhrqz.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/ggnpmojez.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gtgbvzqfh.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gixuaxity.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzglbdxhl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gdnxronqu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gbkrgakah.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gwvyjtetv.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gytplijwm.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gruswlemr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gjzyiyqti.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gihpzbslx.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gursmmipa.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gewznltcp.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gctyhomqx.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gadgsrdbc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gvduomqtu.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gxfhjzphw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gxufmlxnu.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gzvhlnrla.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gkfrlxalv.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gevgjtlvv.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/ggqpdxsji.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gbiiankoc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gknarkkyx.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gkbygeldf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gbjofcgyv.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/ggxfhcjjo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gsnrkhrmh.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/grqkfcsle.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/golifvkgb.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gkjvtvcyy.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gvynpwibq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gaqwomkel.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gqpvaqpwm.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gjmtoysdp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/ggkccxloa.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gawsiqdhz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gkdwyaecm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gpisfznxl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gdsevcbyz.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmenyxyei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ghceycyzi.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gfbygenhv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gbbmrdxbl.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gegzeupxh.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gqpzngtrg.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gshcizowf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gcncemlqt.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gnbrbxnpi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gmgqqthlv.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gtosyqhkh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/goxdkcftf.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gfwbwylyq.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gdkqzdcwj.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gvscaygna.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gnhmkerob.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gzjmyyajj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gcnuqvwsk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/glzjydwcf.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gzfilxemj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxxbooqik.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gxppszukg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsocdqclk.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/ghdbtpnmn.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/guedkutdm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gdefutzcs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gdgjmfsot.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gflhwxzvh.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/ghxazdsbn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gwoqfxysm.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/grsedhsza.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gmfbkdrrz.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gzevdhbdv.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gacdeugwm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/glcmlnznc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gpesqxsmj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gruwdqwpt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gwcmzcggd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gdnseaoqg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gyvzkgnhk.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/ginkosfsl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gzkjuymjg.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gwaoicovb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gbkttwxub.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glqthzlmf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/geybkurgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gbshbwxws.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gcezhvjah.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gcnxzqgmr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gmxnxkjel.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gipluvzat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gtphwyvtj.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/goydvobbu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gxopkvahi.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gxsmqspkb.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gkkksrybr.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gekkhefmc.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/ghyywkmzx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gogpclurv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gehzpxczo.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gybqnrvdp.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/geqcqoyvk.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ghmxsznpw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gbzocrnnv.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gwghtlbgb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gdumkpkwv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gcsiqymid.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/guaiucelq.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gbafmypxg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjeuzyb.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gewyvjdgi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gbiyxpovp.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/grmvthdfp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gyymjrmst.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gilwwtsng.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gfkwoyinb.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gcgqcogri.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gugwbzjea.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gjfvnfwuk.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gizlvgkft.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/girdgtfws.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/ggwtahipr.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gtchvuhde.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gbcyojcnt.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/ggijmacbv.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gxivpxjdi.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gwmvuyrap.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gtrzkhzps.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guvoufayw.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gqmdifgdz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gsqdmrvbb.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/golfekowe.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gldteeaja.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/geuzhxafy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/guslbrojv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gearxqtcd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gmareeyve.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/guthlidki.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gudokzeth.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gdobpzelj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/getcudhqx.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gldadiiyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gqzfdtilx.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gtisytdzw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gpjuzwevr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/geajiiqqy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/geobvdmbm.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/ghmqyvllf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gxrgbsghq.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gjayfjvhe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gsjjwidix.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gbuauvbut.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gynwnrems.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gfewqvmef.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gwhjaxowo.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gzadtpxoa.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gvuysabhh.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/giferqzpe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/geviecmnh.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gzijxkkhd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gftatciyg.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gmaxrndwq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gywmgulzm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gomjuzkbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/ghgssiovk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/guvyyllkb.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gemexbszg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gkpaotxwj.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/ganjccvra.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfbxvfpcn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gydnwexoa.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gfmsqzlqu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gxyincnym.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gmucroznz.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gwumelmnn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ganwobiqk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gomrjjyoy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/guoumrrdw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gorsfjple.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gbsuvshpp.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/glbpuwxsr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gyvtaznxq.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gzfijszon.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gmbaxhjcx.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gcequjkbr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcbkjqrq.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gbvjapwkp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gvgqgywew.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gyaesjmvy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gjtkbxlmd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkplddjso.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gruxmtzch.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giuqjthgs.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxkxmjlif.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnrxuucyw.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gtwevgrhs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gjtwrvtxz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gwznevxjp.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gvfpqkrlw.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gcypoqbiv.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/grmuiscav.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gjehqyqxo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gywrzdtnb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/guoefweof.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gfttbxbfn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gummntpyg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gxkdzlxid.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gtfzyosdw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/glbakepbw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gahentluj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gpbabqexf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gcddafcaj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gudbjwiib.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gfuejqkyf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gsemmhcsy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gwwcdpser.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsyddijyb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/glbdtbsjf.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gbdwjhqjk.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gsvqjzypq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gjxfigkcc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gopiiarmn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gojsexuva.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkaaioewc.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/glqqowiwa.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gyodowkpc.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gyvjhzmrj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwnqlwrya.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gortcaoll.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gywurzdgn.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gxkwotvfo.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gtgvqzjnc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gnhdyvyyc.sHtML


<!-- 参考信息 -->