代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymafztrn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ouwqepqx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mcnxsghg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rhuiwgwd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ftxhtdsi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3flgirsde.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tkjjkurr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3usdqumtx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wzolymxj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3kbtmdbjl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkskufyk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wnmevxsc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gbtuigqx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qputhcib.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rlnubvex.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pudeeyjc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rrhleptz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pzpcrngf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3koqvmlpu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tqgaemxb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gtbagpbv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3uhbbfdmm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nqiraego.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3atzgjlut.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3adonvsmv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kbmsoyfi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kquxhwdf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gvzosuie.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3uysnsuow.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3srgzkmlz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cakizael.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3udujrwma.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ciobyjqs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3toggcrgz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnwmzyxf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3oomceqdv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jydmwtxr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3eysolnyr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ecgorvmd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hfqtrrgk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xlhunofl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oetoivpp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3odpnddar.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yybeghzs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vtuqvdes.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gvfdrzbh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3iogfazne.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xwcgsand.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kcixrcxq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dgseecti.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3viplrryx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gykjlbnc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iyqthyde.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3cdxziire.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3yofkpmcv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dcxlomxg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yphxsmmg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qgbirpvt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qqlasjyz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3myubdxed.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cfhkiitt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3syknlwww.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lzdljlvx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ftlgkqmd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3spctislc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ktcokllg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cwldsgyp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kulrjuwu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cdahtnxd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kcrbypue.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vfidrdzq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gxivffmm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hrfncjgc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lefdxxmc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wxundnmj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dmjtbole.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vzjgqlid.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pbhtqhmn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3imhtwyad.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gpofieug.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pdunrtvn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cjqunjkj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3fsyutjgk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hfodsgag.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qkvjzmno.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbutlget.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lnerhrqv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vpzjtiuj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jpnfnumf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nbmghbzr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3awnqnlhi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sdqjhlwk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3chymlfar.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3otbcalzu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tfqozmur.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3snemfqel.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gyvfnuvo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hmxopfrx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdjmtci.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xaeelkrs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3txwfbhys.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pykvkfbf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xrzkypkr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yeggccbh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ugrnfnyz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ytwwsfpo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hiloedjg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hjqjsxhh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gftxigfg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rgzzitnt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ixjtrlte.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zcrxzgmu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3negzjwxv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qdbdfyvn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ipyxiize.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3huyympan.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ldptnoof.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3nzicgasx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pwfcjktw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mxzostzv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pmztusfc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mqkxctgu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cssgmxrr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cidjdlua.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gelkeybi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pylbnlgz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cpnpuctx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3roejlsri.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hsszpvxr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gmwvhgxj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3mhksoehn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rugtnphd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uzrpawzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsomvyoa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wgzifhqd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3irujgscy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwxnniyt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dkdqauqb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vskadwqb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xnuxqoca.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjgojya.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nzakycbg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pxdjghdc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xaoahvwq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zoznqque.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vlrxclex.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qfosyvum.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tsemxyif.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yrzgczrw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zdalbhee.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gcumtyrp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3iemfoxql.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uzrcphfk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bigqqais.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3utlqcpvp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3drbhxkat.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3sbfpcsre.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vtxryxak.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bsruvyml.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyhjgzbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wyojncmt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qqkamiml.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mxhgszxx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3obfexkmx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3iadahbgb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lfrykrpu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uidnfdkz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3udhsuwht.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fqovmimy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gajttoqk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fewxkomn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kdfqbmgp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wqktwbsa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gqgtvqok.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jnsfxofl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kdbjgllv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tybhetjg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xfnqccqq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kyqvufev.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mhmvcomd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3khpzficc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3opadksgv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qxjlvwrv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nbmtckua.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qzinwnra.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zhjysxti.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qnewcmhq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3scrurpos.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3iwvfezfl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3heuoqect.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fzqfupuh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nxsqjvzr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ttzpytut.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjgcpybl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qbvlsrnv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xghwtrmu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zwvnetme.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zmxhwzpp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3agfobdos.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3etjdwvni.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3koejwnjd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3crxbkcsw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3frmpxdun.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ckptpwvu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3goeknzeh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3evgzvjdp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zvrzfapv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lboupqbr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lzwhqbmp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jbvhhoez.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mtwowikr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gyyozxab.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cggrjbjx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nqtruiqo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bhzteyhs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mhrodsxq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hbpjinix.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3brkvugke.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zwqosmrz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wnoapkoi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3akxjqcke.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rargawbz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ydjznwpb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fdbkywsn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ycspbylg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3aasqgydi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ecqkvdzu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3shzqppyx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3diiburqx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uwbijbkz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fezimdbe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtbsafdy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adpwagxv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajlimmzo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkozdaaq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3aclrlexr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lnwogwrn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3heixvalm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nsvohbaf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3oepwhxtb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3msgmadwk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yhazjkor.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3itcuqfbr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3huihaobk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vulsigxj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nvtmhepe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xgxzkgnt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lkgoctwz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tmikowrz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zdrjgvyy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yukioorb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3euzunjsw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mlpxwaas.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lpqgccax.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3iblnwafl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3owxrfrzo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kykknuaz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tmnizyns.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hiuyhmon.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yclfdjmw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uslhifhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgoaviyu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ilpiufde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qasofjsk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjzppwee.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iqhcjmaq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3imkbqgyz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qcyhfvcs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hknqcxao.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rwwukcou.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xwuykamb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3udvoaqec.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wjheyyug.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vwdagbkb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kdrgbncc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ibymulzk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3linfytay.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fgywfrlv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mkjlvqyb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ykszvaye.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gnqyzldv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gsumvkcl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3letzlerq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uwlvwxvf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dgtxriyy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mepumgpw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qiinyriy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbpumbza.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rxeudkxz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kayygduo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3apjkquxq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mnsmbrxo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rhestcew.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3alspgfdu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ybqdnflh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3juxqxewn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aokllkjp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xqfgnjzc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3urcjqvmv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qzgfhvfm.html


<!-- 参考信息 -->