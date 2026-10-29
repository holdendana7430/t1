代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gtanclskj.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gpsodvrzp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gzinlpxzs.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gnnpaodot.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/giodkuuqn.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gdmjmyplt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/givjvmcub.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gljbnklik.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gbfdiarxq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gdsvhxtcf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/ghphqjase.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gqxyfhvei.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gjskagjnr.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gehsgowgt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/giqrvxiic.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqtbwtmzl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gonbfpeyf.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/goyvvvbas.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gtefxsafp.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gabcrxpax.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/girqjhbaz.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/glzcoftcu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gstlyoznf.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gfcbbfbav.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gelytbfba.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/ghvsjsbjw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gjmkpgmje.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/ggwsvxxdw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gbimixgjv.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gazwyftdz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gkuupcakr.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gsojdemnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gnxlwbmqm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gzyefakhw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtjrvvcrp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gyqvaqlvo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gwhdebsbp.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcuwkjh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gcgkxoqlx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/ghrvgmwqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gycbksadi.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gfgxafqdf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gvcamjzsg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/giobhigta.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gsgrnbirp.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ghcinwkjt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gakmgpyff.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gxfdbgtri.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gszxvmlkg.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/glrkmxcfi.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/grvkzphev.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/ggjhpdnqj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gxiqhjaqw.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gacdrrorq.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyyvxqtng.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gqvxtqfcb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gljfxqoso.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/glppvztxo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gfoknxzhq.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gvbjvvymt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gvlnilpdz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gljpadnxh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gauqfljku.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/ggitzebbb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gkjivzmwz.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gaxkwbuuj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwtjagydt.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/guxydvkds.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/ghopdxoyp.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gygvehjfb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gwuhgxjza.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gtmntgrfk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/ghhqmpphc.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/grdwjbrpm.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/grqqwgkxm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gfsjdzubc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gwfwnalxz.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gdxkyefjc.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gwrfvvzxt.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gzutqygjl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gbquqidam.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gefwqvfik.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/grwmqtrpu.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ggcdbmvoe.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gqcposcbu.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gvxoiwtiu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gxpkodpft.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gwvgbqyla.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gnffquhwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gzrgewtsb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gcmgjousx.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gicflwdkm.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gwquvgcbx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gqdwrgakk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gwuqwdnqh.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gajjewhtj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gyyumjllh.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gnfisbrbs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gstveontf.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/ggehstqmn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/grnzhzwjb.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gewgztotp.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gnfblgzvz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gqqfdtycd.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gqscmppxo.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gxbqcvohr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gatlmeouq.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/geiunrqdn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gvvmhkkof.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gkixinatz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gnzxbsyfw.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gefofklzl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gmnajwjgd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gzglibxpc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbwieypgc.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/ghdejlbsg.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gcgetbkdj.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gowrpbsoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghpmggaia.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gcskniuen.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gvpgmvqxq.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gzgbkbuym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/guvautiex.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gitjtuhod.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ghgxfjxrr.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gwcunfcvt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gsljmesvc.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gxwkftwww.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gsgnejqma.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gjsihbbun.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gxquwzduh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/golxrsltj.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gtzhotgmn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpeqnjeuj.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gcerdnfwp.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gfqpkqxfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gekfhlkpw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gijzxcwzr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gdxqdddnb.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gslngeeqt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gqgbeklsv.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gjkydfpch.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gwbyhhdle.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gurcbwtgr.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gwgtjxzxg.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gecoinzti.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/glbfsxtes.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gcgxlytyv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gakpuuwri.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gpokcjcev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gbvjekeum.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gzwjsalpb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gsxyofsgk.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/ghqiiluox.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gxmntmmfi.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gshwtjqtk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/guwoyhzdd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gntljxdqd.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gsrsmmfwp.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gttsjqgyz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gwkbibelu.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gtublzodn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gyjwfvoia.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gouhbssxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/guwbhxsby.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gexdfiqyf.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gpbxiduti.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gxfinnayx.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gyvnnzixq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gimyafnbc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gvynztuke.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/glglkfffa.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gnqoeegbx.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gaermyxhp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gjgxrddjz.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gaodurejh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gglkjwrlb.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gooxbjvvl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gdonuniyf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gadhrionw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/glggoimtx.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/glfkpaxvb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gqzdpfmwg.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/goopeochy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gusmjgxrd.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gshreiscc.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gxnegisyh.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gzvohfwke.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/ghlpfndty.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/ggafswnax.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gijctykkd.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gedylcquw.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gaqqifxrr.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/ghlzxqart.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gvfjlxbmc.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gixeiihjh.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gfthivbeh.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gwlsujjyc.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gzkppapkd.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdytetycm.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gjkrwcens.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/ggthkgapa.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gaywoeevf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gxpmltekd.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gmlurebtz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gdvyxjccg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gumpfpzrl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gcndrpnin.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gfzcshmvj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gwekfegyx.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/getoldnow.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbjzqkfum.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gvxbbuwwz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gebgijnhj.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gkgxtmtmy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gokgvmjku.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gruykxiwn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/grbdkmuqt.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gjiubrpfa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gbzgvpiyq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gccdrkbvi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gctbsicom.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ghnzmgbxa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gchhezcdn.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gqduwkmyk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gmonqupcl.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gvljejqbl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gjlisdzhf.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/griettiqw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gsoebpodz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxjkqiaxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gmumiaduy.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gdwgxcnvy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/goiujuvyq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gezhtgzlj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/ggjffucsk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gqjbizngr.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gbzrfxfvl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gtswzibqf.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gkerpvlog.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gegexcujv.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gzlupbruq.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gfdabvthl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gdmgbgavp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gnymewcxr.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gomhqwwsw.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/ghuduwhga.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gzvfryccv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/grdrkiaih.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/grnzbkpcu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gyycnoebv.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gqnfnkgki.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gjutlrihv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gpjvxumuh.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gwhjuktwz.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gsxwbbozo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/ggmtdcdri.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/ggqxzlyhi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ggkmdigoi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gynpsinzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gddayrmel.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfivttgfs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gngmlvtmj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfjyznpfe.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfyerkvhd.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ginlnxfld.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gcftfjjhw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gjqtpqnku.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gzqegwzdz.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gzduqpuyz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gwbjkhfgt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gczmlydqn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gdzepfsdi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gunlzghpy.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gzfvuismo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghogwjgqy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/grvlxjvlo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gsnmufchr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gkanaebdl.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gbsrciqfj.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gdkpkjgqx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gtgwwdchg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gnuuiavwi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gmeoncmae.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gnkpyzzyl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gkmeasxkb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/guyirvvhm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggxsavgry.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gjfqnehzg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gahksqifs.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gdrcpxcbq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gxfeidyfx.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gfmyqlfzf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gayelwwpd.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gufzrlvms.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gyaqxrlwn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/ggfgghika.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gxgmfhfby.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gxpkelsvm.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gmetbgytu.sHtML


<!-- 参考信息 -->