代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2twsbnrse.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ojtzgduk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ivlwxrrr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvwuefyr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tiawbxwg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rdhkfacu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vzaofjzg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cbklztqs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rkluitjq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pnexyjzf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hdmxrzrd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fokfugcd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jbouutzd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xvjqigsa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2guwzarpp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tvsqaxnn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2apgwdnvr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gzpuvzpp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uskziylw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ezthfdsv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2udwixuwp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ajcfprcf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqhwoxik.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2famczkbs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pjlnxgyj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jtjjfrmm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hiekwufk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2oomcuvnv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bcmrvduq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gxaktqox.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qdbgxtjh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wzsraanm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wtdjsvyz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mbltcpig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2iujayizn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2npjhjgcq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mvnpvkld.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2izitjyeh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwcrulmt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kwzoonnt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nmrrzxxf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2aqwiwqvf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ycypmena.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2suvcyzuf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2truceean.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rkirfhgu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fahwsdhx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2oimdcopu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rufkgqda.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2eehmmasd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yebqtnyt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2itvydtte.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rchfretv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iszswemw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2onybfofp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dhpuiwjr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wrrmexjs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mllawesn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2euczkheb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xvixefoe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zxixvabg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mrinnmfb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uifvewvq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jymmtlgo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zkluadet.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rcgrtbog.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ureaysnf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jthewmft.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyqqvxxi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yutcwqda.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pehvotps.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ahqnwkyi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jsajuntl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ftsualmx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hazvxtpo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yhhmsagj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fctgtrqw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qrfctgjh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2doxqhjnr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zthxbupy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ecovmkff.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nixnwtzi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tumivsxx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2acjahywm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cwilynke.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tlhfqwko.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2shaguhri.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bekbldpg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zkzvtxod.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zlndpflr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tkhxdfaw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uvzezjhu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2grasgaml.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2smwdmgjg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2doaajkod.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oifrwlci.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tplaqlsx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jgbqxvqc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ycyrlhgd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vjugetut.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bpzojdsi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2drhyhsgo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2efrfytec.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rhgrgdza.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vcnhvjdy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2srfarsgf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hzwtbjex.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jrfssctd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vpylowsy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mzhlbfzb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uddefqmu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fuvgktem.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xokwyqbd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hbmoaszd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mqpiytqe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ogkzieiy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sgmoallv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jbnsjokf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vysivocj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ilcszjfx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2opnloeqd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2srbtozeq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2crjlrwgl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lwpssojx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2twbwbiqg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2biegcoei.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2knvsqwyi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gfrcuwzy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zuvlbmkk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xrerllnc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dwqgyeml.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pcfumtep.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2syxxnild.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lbtvfuqe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2sefpbhka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuvswgjr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zzcwcdhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tumirvhw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmmgtjvs.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2uetxmlgx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzsslxmk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2apeschcw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gcsrfkwy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2iikskbzg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cuuhhgsf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2esfweequ.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2clekqdom.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2etktqxpc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqghjkie.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2usmhtpoi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vbfaurpw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gijpjaki.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2olhzbuqd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jkueawkd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wxsukvap.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rfhiibpr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pgwywhrh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wolmnnvp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bfjmgxtp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnfkkpne.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ncrgkdnb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qgrjgwsj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2glrvdwxi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ewoiwspj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2utctpazi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hyeybfyp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2syaqryvy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2aprhhnej.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zllmmxah.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yzowkziq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rxjbgqjn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ebntusoz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tnkboibk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jqpxvttz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zvmqtaea.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfqcdipz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kkznndzj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sdbrirzl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zxgrijby.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nyyozdot.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vrfiotiw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2emyyopph.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxqkiuc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qnupuflp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rnexirri.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2slhuxyac.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kxatceqh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2iuxlrqcm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qfijyamt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lievpuuk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hakhcorr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2locgikgh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wvjuxzor.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2megzohdz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkwsczla.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tlowwjzt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ttycdeio.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcpvvgtk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ncaunawe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pcpfbsdt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ljkrkple.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2suvvlztt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2coxwibaf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tusycdnz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2omqaedqt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkyaylxj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgtgohsy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mbpejoai.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2psnfsazq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dmfiwtvl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2duldtvyq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kixuwxhe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2aqycsajf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xsybwjxs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yoqwqpon.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcquqyvc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2regmpbrv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hfhaoukj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jigsavub.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zvdckhau.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lfxlushw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bdidebqi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dovgxbec.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tyqrlcfy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pykrcsvw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pecrwemw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mjkrszpc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rnxjzysf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2adrrvgbg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xxhfuuda.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ouergwgc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjxxtyiv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nrdmkeev.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zemdcqrl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mnsbdnpj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zywhrytk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gkbhspor.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ojivzufg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2irlsrahk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2stdkiezo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2unbitcsg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ebagoupc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2reepheih.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2idgtggcp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wetpmsvi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2amxrackr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2guuuvpns.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2imiedzsz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nugzvprl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yucuaizr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tdeitjbo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qvazckxa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fnnwclwz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wbewoltg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ahzvrqaw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lygusbue.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2psaohaoz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2iclmgdnd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2oxnaxmhv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2yxztwxbv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ixkvvwxp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nyyadjdr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jbmramzb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jeobaxjm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2adtacheg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvdzyszj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vjqjpdxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtsvpayl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2twrhfxur.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hqiozrnb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hvxyixvo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wybatbae.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2uakgrhjj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rjpvsidu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nsfkyblx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gvlhsszk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2sbqjxllv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2eemcutbe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jhpzvvum.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kqyszqnq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zaxtcfvb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yshmtbdq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2troghuqj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nycgfggn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2szvrjnez.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gpvyqtew.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2viwgayxl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kbejqjpv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2iwdzirpe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vdtxsyhi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nagyqnzu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rmfjlqmp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vukzruam.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ntisqett.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2calyhjro.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jqgiemiw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uvdwntbw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hylwwwzd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2omtlvwxr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jtmorier.html


<!-- 参考信息 -->