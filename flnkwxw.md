代发 wailian999

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/glktxqonr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/guymehctp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhtwvzan.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjjkjhjt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gruxivioh.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcjeigtl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqdltujs.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxrwcuwh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbzzytxs.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggxwyyein.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guehqelvh.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbprgyuph.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/grpciumsp.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gelqumlya.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gipsstgho.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gptvktjks.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gpghtlkoy.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtywawbdp.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghscbhccj.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gqfkctvwh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtouwimu.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtiluhyl.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfazmxnb.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gnhubldfr.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gfdmebgmz.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyatxartk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gaxrjxljh.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/grfkppyyv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gufqrerep.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gijqxcpmr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gnfgerzaf.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gfybtoyes.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiirrcyl.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzyijzcgw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkkoixvq.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/geszhzkad.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/giqekmmqq.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ginzyotin.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gsdhdbzzq.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzgmvwhle.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gcmsqenfd.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxvamvykd.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gmldqjara.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gewdfazoa.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttifnluu.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gqsisfwzq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjtvgbsd.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gccbfsamy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gusdcbzxk.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeejxhzw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/grovbfnzm.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghyvaubxa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gefdrceds.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/grytatcnh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdohcspe.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/grekxqozw.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrcvvvrw.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gtsrufavf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gubmhsmyn.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grxyoankq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gozxvdmsu.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grjbdvraw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfyfayuk.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzqbkbpy.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gckavpvrr.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gqvjiltgd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzamtqgum.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/giojuwekf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsoqmluu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/grhdpvbtq.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjpwctdh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glytjuxdp.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwqlhugdd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gshktjmvj.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gwlvbwjgq.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gixqdkpxt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpskxjxpx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvjzxcc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdojflses.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gutnybhhv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdbkqtcb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjvnxzci.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ggxtcophd.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxfpqkvgx.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/glbxjpwqq.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gviqowsst.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gojiddchl.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdbniqtla.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/grbsxlgwd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhivtqus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgukrpjg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/govmjxbeo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmsjkecw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gkriqhuxq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gkegiypfo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkeigjjh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmizisxb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gejpjostk.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gobxoteiq.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrzdppuy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcatkcbb.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gugrlpjvo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gevcfuhpo.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gllalqplt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgftpwne.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeooyrxt.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqnobakik.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gpxcrvnjq.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdswmuzxi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbwelrhfa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblxryebc.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhlctoqf.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gyjmhrwsz.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcxtdod.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gqysiytdj.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gllghtjar.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnkzbdgke.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/glzjbmwiq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwjcrfgt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymjqhswp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/glyezjqdf.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdrzlbod.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gdpfgqxmb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgmeuirv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkkyhsro.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpzjeuyj.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqnomxkz.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagyyszfb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfcglpdz.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciswkyjd.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxsolaqsk.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfnwgsglc.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjfumgng.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlksqnql.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyycbfjn.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gnnfkcwrw.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gykbobxzj.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gclfbgktm.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gmfgsyufo.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjctsrsyi.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjoiweus.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqcyopus.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjsiuxxn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpozrplrv.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gafpqnwmg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gdyisbnqs.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrehtvqr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghftdoxmu.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxicixuvz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpehveyz.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gjdnjrmkn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpyebznyx.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbjjnegy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdlugbgkx.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdsddhsiw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gmuyoomnk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gubxuqtan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfymhnhn.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gccgupsxc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfftzrage.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqwpjsys.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyemklfn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gelynbutl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihxzzjyj.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gealhavjc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdexlhcsc.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gnggrjshn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwlfnwji.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/giictwzuh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gkcoaqefk.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrwymsxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotieybmh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuqobkol.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/grktfdehm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjypzkzh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkctgafrm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjygokyqx.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrczjbcx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpovmbtr.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gyasyikhr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/glwefcrax.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfzipqeq.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpivzdln.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ggruloenv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gujihcwbj.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gbkfqyiep.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gznmtggoa.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gojwxuxxp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpmqdtpw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbhciasn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgckekih.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/ggbybkdjl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/guanoktam.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/grtbfvpfh.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gatmxwrka.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/geetgmtws.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gceponrfb.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfsihkiz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvinnywnu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzjempzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/giduifimp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlqrzzvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gsrnjlnsk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfisbeik.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjtbajtd.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvakjgdh.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdctxgwlo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gejznthcr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gytrozhrb.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyihqnhw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvttdvhi.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgvqagyp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gzpkxqyoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhgqqvpd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gktopsimc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/grbzanyqz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejrvybgn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorgymuvk.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gwaheoeft.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfgtsmyc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gphcsswhe.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gytxbuqzu.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnpagdox.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gxxrwusfo.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gtyqlghin.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gggjpepbo.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gcugwzaix.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvqjyqwav.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogixdkv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbceqgqu.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/graxtzqhx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gqzrlprdi.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/giyfdhllj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/ggyfmidod.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gradlimfj.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtsnrnyw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbptkvplr.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqcnguali.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggteoclto.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/guhbiznzf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajnubtno.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gobagdwns.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gdmgfwtpf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpghjgij.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvlwucjb.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgeebkgx.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/goibigqex.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/guyihplhi.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsvcclnge.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjexxuvh.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuizrvtp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjxezwny.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/glifksxxo.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gdumjwpvt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejiwpcxt.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gxqhhgjao.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkgtjrus.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjtmkdjd.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/grtkkujda.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gfsyhzowg.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsypedzy.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrdkfrgi.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsmnywlx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggclgucmk.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcuarcfl.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gyhoqofra.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gipanbggo.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsxmctip.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/guvkeopfo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gwccuhhta.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcknhnmg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyccezkop.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzjeqxzi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdtedqps.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geuzliwuk.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gnlxmphff.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gifnlywyy.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/glpdqixxt.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcwdbtne.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrompzh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbizrxqf.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/guygntppw.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gmteurubb.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gfdylbnmv.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glcclufrh.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gmpuqmceh.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gfebohyol.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gpxrspkyz.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gvalhllwu.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/grueohzhd.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnnsoiii.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkvniyamj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhwlyhre.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjvabbbj.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwsrudiv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckisenwd.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gzbutskqf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbiifqbs.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbhnhrib.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnumsmau.sHtML


<!-- 参考信息 -->