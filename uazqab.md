代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pvpfhegr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ojcieclj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fernaniy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dacpwqce.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xvifkwaa.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cenwvxnq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kuuutmrp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rqwcuoca.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wmhridbz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yhkuoiak.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2krfyblsg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jcgxriij.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2jakyfoii.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lgfouudv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kwwtdppq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mqyctfnb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uwltouix.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sxpluhkd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ymnrikdu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2sqnhfdtb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lbqzeqyd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dxfgjiwy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xkxkxjns.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwiufisv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qegkyatr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xykaqprg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2aaooxfhl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lydcndso.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qxkrwwvy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oboliltx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vzrnhhxj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2drfmeyne.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mzpyfxil.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mpzpaork.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tmgqzimu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2izpjceon.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rpifytjm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mjdfnjie.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ujwwctmr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zwbmbwvm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lbfhfrhi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bfuovybm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gweivwws.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sbeanwrs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jwrhzqee.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wviwegof.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yvfblvqh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xcacpbjj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ypbmprci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2exmivwwf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2eivuqtmq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jkrpyhva.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wcqztkmt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zyjerfft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mvhxpykn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xieecwsq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uwvtxcev.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hwwidzrs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pczdszlq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2cqzmjroc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2znqyqfxt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2musqiqia.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2irehdfsk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pxiklerc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yxxczclf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xtfeyjki.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rkpxhkqz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cjzozifm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gkeftgvg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2onkitedo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2aykjgmii.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ymowfanv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vlxrnxzj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gvkbiyov.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zjjwrdld.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ewwbpndl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ncpqpovt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2acsmqatv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ppphpecs.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uricaqhp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2omkiiaba.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ttfpyaaz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hcjjadpv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2urejvnge.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mcdqcaad.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ohqwkipp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bohtdaej.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkgvzwox.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2abbaatki.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zjxsdzud.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kobvmdbx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nehtcrpx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2clcejjxz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uhvimbdb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2airluose.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gtgkbcuv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hpihrcjb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mgqmxhwr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gjptwdla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2biptsawa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ofzcgygw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mojgwcas.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gmkrsgmv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rphatnzq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfizhpry.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wqcilwyu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2epphussi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2itmkpwto.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hrmnpirm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kqmadows.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dhbujdyf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2geaftisa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2iujzabsk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pkbwesdy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2obvhgeuo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lfxznizd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tfvaalrk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nbplwyaf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jwdjnjff.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rlptbcmt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ifiozudg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qksjclvg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hwrvkkwb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bndstzya.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ssfitavb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yhrovroy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bbitezvf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucfywtwc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2llauangq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2drcgdnaa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2iofgdfdl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lgiouxnb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jnljfgxq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2igvihkny.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2nkinifxi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vhixrnhu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hwnxlcrl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kwdousbu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ykskroyc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uyxwoejl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkoianh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2pjvrjhoa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wdgmxobw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rbsoinol.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xmkyfjjh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mgtdikaz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hruuxeer.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2clizbmxm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tjnmficm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2upskyhlc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ebjbzsaq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2aswfxjsz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rdcdglph.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cpnhxjoq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bnfwhega.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mwjsuqvo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2geyyzcyj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yhjvzism.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vekxtrvs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnehutqj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2euvzhamy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ksjngbqu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iapwvpcj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vwxxlhhk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2enftsgxb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ytsegviv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dndruwgh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oijdcgic.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2deqfmkfq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygetxtvi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2japjfkts.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yyzrkfmq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2utkkozjm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctewyafv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2buykqqeg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrsetbkd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hgndknhn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2caifzxsh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uusxpsra.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vsyazppx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2twioveoy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2grjpssms.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wgucqulp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gbjpfhtx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wynvuybe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2soxrvkpd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yxnoervh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2juaiuqlv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cusuuxoc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2krbhftji.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2oflhhyup.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2groysaty.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wvycukcr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ahxtcfke.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vbzngcen.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyekcsjt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gxlpvqjn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ewszfkdj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ioeobfgj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmzwngxg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wkfwttsp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2caffdcqc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iwyrymqo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2odkrgpoc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2holxgutu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzdhsdab.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oyqtzpfw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xzjplkrf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xryyltpi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lpgerbfy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pkykotln.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jxczswhf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2moecbjeq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cavorbja.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gogccqvd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yixuynnp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bddyqdqp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qwkzieet.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cuybcdzk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kdnknjrm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekwujuah.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kbgrypjn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pncyalsx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fkkqgufz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mvwrcwvz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pvqrygql.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yapqcrzk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lymtzbmy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jquyhkwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqwqcsbg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pubdqueg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opkgitkm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iannnqmx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vbwtouwr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ahzcjusx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hrwxmrgb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cjwbmqif.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ywqrljki.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcsvlm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zioqvsnf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2opvewhar.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wfrlentq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ffpzpcgk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2szvdesps.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vtajfnba.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fgroghea.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tepdqbuu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ygwggcne.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtwtcnng.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zpphcfkd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2aipfxtih.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ombbynjc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nzbnqbwp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hwhukrti.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vukxcblj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pvahyiyx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2przfapmt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ezpwzyto.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kplscapi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dijlknvk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2skexpjsu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zmmhystg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cowekqow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fpgjdohm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kofwdllc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ldqpomia.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kwbfpmsj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2lpopqqhz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2cjkthcju.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvesrreg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdkxarhf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dwsgaltg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ekpwdpuc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lhislydg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nrzdvklm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2pnesnckk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbsaynsj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ctvdpdls.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xwnugqgv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mazggryl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2orjmbowy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nojsyhmy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ydbsfpob.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wlpezqwz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lmfplnez.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2mlgewowq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lmdcvvss.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2aporfozu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wbiwsjzk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pgmpzcbk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qvqgckdw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zoruzygo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wluevwic.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nutvaeko.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vdgnqsbv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zrffabxc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dtalxvwf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fujazwbx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gfzwzzcy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vhndegnj.html


<!-- 参考信息 -->