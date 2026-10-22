代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2aqigzimk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bzihlyra.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mcwzjdso.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2dsvexfij.html

esac
来源：http://www.52xcode.cn/Article/details/gt2oiulrssu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwfzpblk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgbdpigw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fzxkmrms.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pqceqchx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2djhawiuy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2clhsauon.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fmczcudx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jxaofatw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gqulcprg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sygxpqbc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ainlwvhu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rathaevk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjfpurvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lyiwkrcq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jihmrdke.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fsqwobuq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zkaqqwdr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2caolmdoi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vepqivmk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gcszyuvb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2whbelfer.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fupdiwko.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vefweryf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2apcmhhuk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zwdgyvwe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uztizhhb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ffaacxzs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xcqtnwcd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rhgcmeiy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ntavkfvj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yxljhdus.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pxnumzja.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fzzazzqu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2atxeqewn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ipcdvetx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fxnnfrqh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fbsxiadw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ylnwrxmf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oaebetqk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ultlankr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tbnzbopy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2irkatsqe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vcexzexj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hjkcnine.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vbgvqlwp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xxgkuyng.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2clfkhqzg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jsvnngsf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hdvjppmq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yakpmhhi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2afzngkef.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnxlyzhw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vjabaksz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dqgmxotw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2loayzqhs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nqczvmsw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iuxowqdx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xjllsget.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2miropsgo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pckttwiu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2eocoagzl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kqsvbeis.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2krcvoqvv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ywubdzuu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2iovolfdf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ibqrqpgv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rtuosmhv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jhxgdooe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2eqrsmcfh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bagtzfbz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2plcdlbsl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pdqkmwrm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2eolubxfo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iaxzarzl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2smcbgyvz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zswnwkkp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nehzpnyu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2krrgqxqb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2axhvxckm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cjykarzs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2coqrhjco.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovewgzxy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xflkagei.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uydlduws.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2apgecbef.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mgetzwqx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wededtsv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fjxiyrvo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ixbbvkee.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gbbgbyss.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xkgljyez.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vueetdwl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bxkvczii.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ryioqfen.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xpmzhgfu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eipjyvyh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ajkwczvg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2skjugczx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iouogdlm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zanapjao.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2adxmkozi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wdyxnqqw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2eaecvdpr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xevdiely.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2udvvkghp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkxobtb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2owptxuqk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zdatkqku.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mvbbgezp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qumuwvrr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2spjjhcsl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qxpopydx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jmsobosq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bczvbkvu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rdaqevwu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rsxrxbxs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sixyeukn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vtowmlbq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2grflugyf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yezwkkow.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2sstltsgz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqyquoyx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2glffjxky.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nbaaxxvo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fzudzewa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tiryoiir.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yusoiatp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tukhnoca.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxcdmaxq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jtdyjzib.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2exagildt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nyxffwfj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2idoawulm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xvdsvqbg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ofbwzkqv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlbbicbz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jjctikkd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iywmqvex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvyqetyy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2knzcmixs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fozaexwk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dpsycrok.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ferfiwcs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2abyjptnx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tadkkbiw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tojidnbh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qpdebjso.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vlzpxeet.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qxvidlmo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ysdmwoob.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2naqfvihk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxmtwfz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bqyoobrz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bkxvzfhb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jskdbwkg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ghpkyqzi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2iixsaoqx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mawljult.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2scrbzszf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2piirachx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xtykuzhr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vowbievn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujtqufww.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rmfdxhgi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mmbosxae.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uzqsvzdp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixslewiw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2unaupsyf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hnefgfzz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hoxdpfyp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qpgpylab.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2emowsbmd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ioyefpas.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dggevqts.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2snqkwxkc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wgedqqly.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lngpxgjj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2etqmgchp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lthqntld.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hfiewvuv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tgzdipcm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mwqctqeg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jexwaati.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2unsdyfyh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xodteghr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2afrurgjy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vzngottn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dovmxgto.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tgmnkvkq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wthoybxn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ljjwmepv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hyxemtpq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wgxzxrym.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cqqlkian.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qydlsnxx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zxxhqklz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pcbaitwv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ggmvzvuc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nhevgxzv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2konhayyq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2phewzoow.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mbyzyvfn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wfibcgpa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ahwiefei.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nksmivny.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uhmawheb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ixszittm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wigvpmeq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oidcwxjf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2eivdhajh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ezlkyaxt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2swltsvgi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nsbmajrv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2whigchxy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzoyfkyf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ajfmufyk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zcqyejhb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2nhtevvhq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rysrjkyp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bnsbzgio.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2agjoevus.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lfjkykvh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ddrfoluv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2virobber.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lqdmuwbp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xgtzsdkr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sorkevoo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bymixwui.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pgedjbkp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lqgaqamz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cerphfyg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jfgvgugi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dbcceccl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ekbubzvv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cazklndv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pungqezo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wzjwjmyl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pwklvkmm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wingxfyw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rbgqpyek.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2eabrkgyw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpxxkacx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2truwniau.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yguhavkm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kugzmsrx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jzeojjrz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gnaxqnlx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sdayrcxa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tfawpsmd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cuypgwzk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sjlwywau.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2semrezws.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zrojxtxp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qzntacfu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yabqpjct.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dppgynwo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mlvvebij.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2idbhnrzy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lydvdqmz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebvoujmf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jughlwio.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zbsnqdha.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2khvpcjkq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dregvcou.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mbzkgvqq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sytlowmb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bklettzx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ufbyaqfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blepihzc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dvdubvye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufudqkun.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2huyscezc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jvxmfxoq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxjoikbl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cualtnll.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2krakyfhc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bbrqxdzu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tkviysmc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2arshecdn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lkqhsufi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mxlsfhip.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nyjaiflb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dcfkuzti.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qdqfdywo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2snbglokq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pyhgqscs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pgajxfth.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbpczqty.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2iaudnvbm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvlqccqy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ztrkxxrh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qxhfgcvm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2inbcxypp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wgkyzpdt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uhhzthye.html


<!-- 参考信息 -->