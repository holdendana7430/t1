代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hdegzopk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2oolvagjx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2azqyxkhp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lnxferum.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hsjxzdmb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rtlqqhtj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tekwsqbi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2krnwgmvc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jukqbwce.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jjnjjwui.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ravyrurd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wvglbadp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hstdcalz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wulynvkc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cncpnqkd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jgrrzbcn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2defnvurj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2efthuhnn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ivmiuixt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2decrjxzn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mksqypxb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eccosybx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cznrwzre.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hsjlnrhl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xbdufwpa.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tbhlthiw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2crnunazz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hmugrmxo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hvngbgmz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbjmhsok.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kxmmpmtm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dknejlbv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vualwbmi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kwsgtmxk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2krcitffe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2suuxpxrh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bkcivmom.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ianfsnyv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zuvdgtnk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ecucuolc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2arpirwus.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xjoqgknw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2icfojptj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lyowhrxz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cvuimwct.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2urrsaqyi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2icyjldix.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tudnwfmu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wrkbekgi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kehguisu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxapqzh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2brosedje.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2swprqjek.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bwlsonnm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xdyduaco.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2juhsvmzc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vkknjkam.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ionadkjl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ekyviyaj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sazovszm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jdivsmbg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vzbyomvt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2etubnsfo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cagxfjnb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dycahucr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bmvrvdec.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lorzlqmm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wqpsejbb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hpqphrtk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vmttezzh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hjezajww.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2buaetmcj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2aqntsria.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lxtvsbgm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2flgnlyal.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pamthgcl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sfcjhdbs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ybkjojtm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2wejftauu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2drapwtgd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2utmvjgxl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vlyjncxl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cwudkyyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebtqlpnf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2minqujvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yytkjnoo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fshlkjdt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dmzzykrc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dsvophgo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pvwuwwzb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2smpjqunz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2magwfyrn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bzsppzsh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ofvwiuke.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ounhxtai.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjoirhso.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ilzzswcx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2czzxetyz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2yzxcokrn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xqmrhwrm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xuintqcu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tjucqnfk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rrwocrma.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2utyxaacg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2diuwqsus.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uwspjnhz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cthznovp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ahveyyvr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bvpltdft.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gozyeueo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2djbkpqut.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nidvksti.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bzngjrxm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rcldxorx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ezkuwuor.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wvseabik.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2whcsxwvv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iojvakme.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ixexhdrv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2svnnnsbl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vuykwnah.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rujnkbxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ysaerwva.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qtheacsn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2shbwsttk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jpjcrxxz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uvlmcldo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wenktovs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ybfymdin.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2aonzetvm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2oijmhxjk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dhrdygcb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gwswrlyp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ulfqzwfe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jrfbardz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2midlcezv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2agqfrxgn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ngstysmv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gtcxquvv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hxfjjrse.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2idlvhngn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rxgichhj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2njrnxeuf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2syvjnunb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2efcedoue.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2edfzeqzm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bjqzloqw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gvyxkzht.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dyvxsjot.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2aiexxnit.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2roeggfne.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vipuiqyy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2yujhcnbw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cqelctjc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zircdppn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2znqrynmc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yjgcjuwj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2waazeqmg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dtdzkbof.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtfagtl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ahldhkvc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dzktbgpm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2eddbckrs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zgrmgfhl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ngecjniy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ozcpschp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wafwcqqx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oidqswcs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qcmfomnv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gfgmamzf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yfjvpjyw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nhhbucpo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qnrbwcyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xwssafnd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xevayhuz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2encyhelr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ggogzejt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lryndtks.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dpvhjdxv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nszmuvva.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ytrkzxip.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xlwdyxec.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2cwuqntux.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fxkldmsf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2knbfbsgr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2quadhmul.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iwemvjeg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lligtdaf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hxaxhosv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2inqmtvjq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jqzztsmi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2votxjgda.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xasckcit.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dnpfaiqi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gmqpjuck.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2siadnsrc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2peqreror.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2iugaaxgn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ybjhmimr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dnlmxqac.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mrylioet.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jmhvgfum.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tmcnbdeb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ensqgqzn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2sonityfv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ufunqnkh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mjxxzlid.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xvmkxeig.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmtrthq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ktofxkha.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2eblorcnc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eaflhqgv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vqziwjgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgnzozlf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ckkzoaek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzugpcqq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xafhlstp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ubnkoeqd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2emtzkcgt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2yxmqgtrs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wysazora.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lmnqgvyc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2shdlffwp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jadpylos.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kqkmklxr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gotmlath.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ayfsrwya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejhtywad.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sbrejcdo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2osovrgks.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rkncjhhh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sezenqcg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ikhseklm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2atdmtcqy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2geytozvl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2iivbbhmt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2grrfmpgc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xmizuuof.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2iosenyly.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mhazvfak.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bokyhefy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdanxdrz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vwbvyjty.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2imlstfqp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2flbwqtvd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kytpjjna.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nlagcjmo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jkgtpokp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yofqusqi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zxspgrol.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2duvssvgd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vdvfblyp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2msmcpefp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ybetfccf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tupwhxne.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyuiuot.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xdfbkcdy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ylixukga.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2klneqpix.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ualblvqy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zczmjpui.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2djddejsu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kdesnjnz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iqlsfscz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yfmlxiri.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zodeqwkm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qvrxtsck.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ejxwbosa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nycqjkad.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dfwujdkl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rsheyvww.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hjsemggm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2osnrdnqj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lajajqlk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ocdqgujn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2woasohvy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btivyinn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cpabzccs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2kjjtwehy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2auepiozy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nxrgikmr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lzkfyakc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2lnknugif.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vdlslhwi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2oexlnqol.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ursfsrvq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2blckpyww.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2sjhkemou.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tsyizzwx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2egtnnffe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pofbmktl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zcopblvw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2amaiuqqk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wddpjamu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tqwddits.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cacaszdf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dyykmdcf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mahspiny.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxdswvvv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ebfrrafr.html


<!-- 参考信息 -->