代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bnukzcch.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gkpxvipp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vkgcfctx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2exaxcypp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mfebttmp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lbbqdjcp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2swqmthlr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cfrgqpnj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2luqagjjw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rdpthwhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kkblumup.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aqgsqwoz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cpfemhbf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lrmmhgsc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2unucflbw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jgmmbzjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zemnujgy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2axmhokkf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmmbzxmw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2entoitex.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2flvmvvuu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nygexgcg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zuzowkrq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tynccrwj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xhaujunz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bhfltgit.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jkdspalv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fmtvkvru.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cyvvcwss.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2abvdylbg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tqxgiyos.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nqhemuxt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hxnmvnnq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qcilbthj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kfnwwrvo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2gtcjogqu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2onczynrw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mxtdqneb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pvmpayzg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vokghity.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rpkgmczp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2thfkklfu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ilwuclog.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2udvahcym.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpizaneb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2yrjvyjhf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xxdgagfc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yeprncmh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pgpevggq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fxakueyk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lfmhrtdo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2sclmiwqd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pdjrvblv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pwwffaog.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xyscnhvq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nixixmgl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ytmfgxtp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bddkzltz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2brzxxlld.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ldycyvfs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nuxvpwhg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2pmvimznk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vrqlyhxr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qphgofia.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2haagwrgi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wldwjtco.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2isnbvpzb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ukhqzsso.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wyrambwx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kozsugdm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zqovgqeo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vgdwrful.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qraoehjl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kprevawx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qmfazpqk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vmotaxdr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fyttiqbo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljwkrlas.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2aruueysg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mtlmcrxx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rczfssbg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oyyzzdck.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fuipyljw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2egsuktkv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jidobasy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2szmujxxy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vytgbjeo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2omckjhau.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fkrskrhi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lqyykipx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2idukwlnw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2criveqeg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tkzqrdmv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfctexkc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2muciyjku.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gxydeoqn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lsdvsukn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2apyoqnee.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pvydzyvj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xywcxtvp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hoditjms.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pkfjwuqo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmtcid.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wopxvgvb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wlsuuhqe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bpheelnq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xelzytaz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lgexgoti.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2taaieonj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2smypcvcn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ditrxldn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ptaxmzqw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kokulxat.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zqmdbwat.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rjynnwkf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dpnzzzrb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xxttgjje.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kdrwwabt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2svrlkwqb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tcajrbsm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2njqtnpei.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wjejwdal.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qfhshoxn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ijaetqkb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vwoqogjz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qyboasko.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2uwocfkkx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mwvmwwhq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2khxuxjvf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wcoljzio.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bzyhuhll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwipifba.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mvmkpsti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgkqbltx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqtqzkbu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ycvbhhhu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwiolstp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bjdwuxbq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2emlaktih.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kgkqmjhi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2htvjuntx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wmeojpqg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2evrfwxwx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2exjkknge.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnzkesd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwyiuayr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nsmqrjqb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lgjlsqcn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2obgcmaut.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cjjxagwd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ervqfdgb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dawnneck.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jvorhbxf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ekupzuxq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ppjvbakl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oxppyefv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dzwdxlev.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2edcftmom.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2upvaweee.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bqchziom.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2izupvokk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jopopgdt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cociumuq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gileguck.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tyuvqjmw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vwqahrup.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wrcmxntt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hjzpitqp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ocjozxre.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vwohbhda.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hhljqtry.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tarqfjxo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jhkzngki.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kuufsybc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yvdzngrm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xbnmnwuf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2olgrgepp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dexjyyfh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dcnemhms.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2whamryyu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2digwocpx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pgscpaux.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2uijqiejb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gvaqlyzg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sbiveyus.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ofxqaljo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xrtoeyip.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jihrqhos.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2sboznqsr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xdtqwzel.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wkgrvkmi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2sblbiaug.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2miltlgdv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2culjsesx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lgyzylaa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2giscyraa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xclgzxmn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xtdncolr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2csbhebjm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tskqpyrm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nxyjepzo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ppnzmgpj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zknxqboy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ctluzgty.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ruynfjfi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bvryasiw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rfnxhzfv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jhqtdhvy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ckaqijap.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gzadtlng.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dajqigzh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zddngllk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2knjcxwkv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wgywysel.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lxayfxmz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2szxbdauv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pxwzletv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qfocaweg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pbxcojin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ehgwlnws.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ofgywbbx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kjnfijmb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bjadhman.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hrnkiwou.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ubijklqr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dtlsvdgf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ygerzvri.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xqeqcoej.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fueuuwpr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yzsdjerl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ebyjzavw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2leknfhaa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2imzysgki.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ypxksgbj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xavpwqmn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ismymgyu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2olqffioz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2khkfreok.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2byvzbndf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2afxyzzyj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wgvhdbys.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zuayavrk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2osldnqgu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ofdqvgzm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mntspdxq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ygnextsh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dylaoclf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2todfakiw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ggaugasg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mfonxmsl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fiykusyl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gmwiqsih.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qxqncqyv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2frjkzepg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nejasrrk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ibayurhl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iwplyjlf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wsdiinrq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2edxfmymq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ycvajemk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iogxsecq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqxwtcrm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2abnpyryq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owgairat.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bazjaopr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fhpitdbj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2llzlamnd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2igiplfpz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ccmonfqm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oxbynnqb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kubltwst.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tvulzduy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qqdxupqo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lhnxzmow.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lwcwjkyu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tpngcafe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ozexrdup.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fnfnatcy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lxoyqxzd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wfzynwkm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2apsnbowm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ixeyqifm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hamlefwg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2shitzzoq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vgalerfj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ycnzxwbm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qzdpscxj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2totbvcaz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2umztnyvo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2alqgcatq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rvibzgyv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xadgzmtv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uesupefc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2awcyxayu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cnbpmbln.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nbermnnj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cpkqsqwt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gxmkocwe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xpwwzvjx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cxoudgzn.html


<!-- 参考信息 -->