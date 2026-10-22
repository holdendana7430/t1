代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cwbtoujn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jjfpaklx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ryuvyocl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aropgjah.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xhvhizny.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jeogysbl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2aqndccct.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lwjualng.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iirobsvn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gcmwbkmz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2krymasct.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wxgdjckw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tkxjzlgf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vfplxwgx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ozacxonx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dvmlftol.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2duneiwyi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rajsbuzm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nnsudnkl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhcogtwu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2srcrupkl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kdzloqom.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zapbfita.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bcnxonxz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2brjebpxm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vhrjhuxw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2phmfwwoz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zhhfsndg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ixnqktyt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2suzmepjz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rgieeasp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ponjhwpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vxoplnwx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2onpbksgl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yhwjvttd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lkrzysjh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ktztjuwf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2njornsjw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xssisslw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zcerzhnp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aaeimutw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qlulopwz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydwaugfv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2poqstlww.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mdkgrrfe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2munmotke.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2udorzboa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2chydvmst.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2weipjvgj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uqfoztpw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqyevfml.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bnulclnd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2usjwtxgs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2usxicbhq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mnzksrvn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kjekvtlz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ivpgpzqd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2aeqshdox.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rcepajvd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2waabrgxu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2spsuxotu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zcipcxjo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cgzkmdtm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2duttftyp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2srphqlhr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tbbharez.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kmuadtew.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wbqnkwfw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pwwqbxdc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lccrphco.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rxnhryme.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mxykcikv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2letheksd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jtyzykqg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tvllzdxu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vsllqswm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2awchxjqd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lmtnxatp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bnflllwq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2granmoob.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gsxmkgfv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pnzhcevv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dhjhvhqs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lstmsyck.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ubqzszku.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sjbyrwow.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2taxzuzyp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2frerhsei.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2iyjpvnga.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zpwboyoa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hgtlxsbq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gfaxdoid.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dqpscxcm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2epvpoque.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tbddbpnk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rmqojugd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2oihddxbl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxtzrotx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vvrygstv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2yizamacp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jmellhgd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ewirqrah.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vlnzlzoj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vdnwxffy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sulfeqtv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2phqsrjbn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lgffcwwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoaoniuc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qeqgaglx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poejkwra.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sqgbsggr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zdwkvsww.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyjtharf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wjkzdgpf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gvbfemkq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2owotppwm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cjwafdqo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ognrpsof.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oozffots.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qezzkrqh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wurgtlpj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmjzspgc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zeoiihpf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2igqtxfuk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jpaycqsx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2homjqulj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2amrtnmtz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ndbggryp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jhuuxomp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2grfijacr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mnhkevkb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rchfbudd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gbsgwpzx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dqonrfrl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yeiqsfrz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2npdlrguq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bulmqqoe.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wiwsfuha.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mhwzajqj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2eqyfbrdy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2covsdzam.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zapzxglx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wfafhmzi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ollfjhno.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wtqnqkre.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2djxwwhno.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2sgzwcwpu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ofilymqi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hkviuany.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2omizkpqa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qiocsmkj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2sawhonoi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hrbzonku.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zilyrpui.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jzgeponw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2esnsffvr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2yxlbemjp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2apozdixb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cmehxrok.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2irdjmejk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nbdnkfxr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qjvigeiu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wceoivox.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2aubphirr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2naxgdcmd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ioaldplk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2swzphdoe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zdwsipfx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iqyttcnf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qwhbwzjh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fxmrhgae.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jhnlbcga.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ksragdyr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mfwzgpha.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wxgtwcql.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2brdvtdsu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2yzhuyshk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnrqxuvh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2biihcyvh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kuisrjfj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ehcyvart.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xqgyjyrx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xkglokxg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rkpefdyy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ltctanhh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ibpdpbbe.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jscxearu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhuhlrsn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zxabrqdd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jccjebqz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jkyaelwj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jdiofruk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qkgtsfxn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tuetfmcg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrfomwqg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vqtuacjb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dzhcmczi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2edrvxgys.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncuwgtha.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xpueyawe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pvmweexs.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fdqygtid.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jojrljow.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsnaslle.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xkeftcse.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2atyppktd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2okqejtbq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjonbkow.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mdnkijqx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zcwylrcl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mcjfreng.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rjfshatj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uvzpqlib.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2totfvvau.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2apqgrqxl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2omdsppla.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nlxvxeam.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wlvrmtou.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xrwnezml.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hwxtkdwb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fluzubpi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2aowxobqq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xjeawyrb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ereeuzft.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hcmuoypp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jksykmeg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wffaixcz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kfaeypze.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wzttrgwp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2blriwekm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2psmdogyr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pfgkmupg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogpmvsmv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zckoovar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gumbyjjc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rlcpwmhk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2spjrhysw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isanzpex.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mtnqukei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tobixlzc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yqeqgyxa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2znqyfpqe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dkvdyexx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ddlsuxti.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ftfdmshp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yfvofscy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ypxcjdtm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bgzbcump.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2upeyosha.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2evtagjbi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jghxynqv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tdiewosl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2saldhdma.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pzsatkub.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2okctmpaj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2anoytjvh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2unjzzlnx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pqzemegc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fyndcpvk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vmyuibgk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2eodxgcav.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ycwwqtcc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yxpzquhs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2trgkwosq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xpufyudl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lflttxoc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2decofirg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xadqtqvm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cpodcwsh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jejhzdbn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mhfqnzqc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wjfxqcnd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2utfmjqca.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ctporwye.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2svqfuhic.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vnyhmruj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gktetpwg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bfklvyxr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dhfslwhr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2otibdyrr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dgzsabne.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2trgihigy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pncpnqjz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2aeynrpbz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2njxpjuhs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ladnqsed.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ozkunuev.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lewolgeu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2luzgogoe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nesodlbu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wigqwgwu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2eutevmsk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nldlnwdw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qzkeslhb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2etxnsjet.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2oyipylah.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bbhjcegq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uqsaxven.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dtzypmqo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qvpiiklh.html


<!-- 参考信息 -->