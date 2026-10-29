代发 wailian999

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gnabwddgi.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gfmmndcis.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/ghbuqlxxo.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gblcqnybn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gedimnntp.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gtzxrlgey.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gynqpnpaj.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gfllfnkpf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gyembnqdh.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/giokmcinx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/glglxftmn.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gddnishvo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gxdelaebe.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gnvveplpx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gdquhcued.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gkzrhzdne.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gvedlzvqr.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gtzmwafgj.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gpmboafog.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/getaixykz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gdttvhzsy.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gbwdnsbxy.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grntlyimn.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gebooviie.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gwtcoslrc.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/geysruacg.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gbfwmwynj.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gnarmeiyv.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gmsgdltbz.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gfpqkkqdx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gxzwiomnd.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gbviranbb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gnezpmpxv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ghqzvghja.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gzgfdxqaz.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gescgjjjz.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gterucoju.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gjgqpkvdq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gbqmryzfb.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/govuuftji.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gacntgjhh.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gxqkfekvt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gkeslvjfc.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/golivcypv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/guavzeuzf.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/guoglxwks.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/glxckukac.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gpxbuoxjp.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/getsvhvbd.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gsfvnsbls.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxztckvvp.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gktttdaua.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/ghirtgcld.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gllplaclj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/ggbzwxslz.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gptweqrga.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gsduacqhm.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gfgopxvfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/guielimbq.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gzhkjeysp.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gorkvnqxe.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gupddwtwn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gwacmvjll.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gqtebbniw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gprdatsfy.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gtlqgxvih.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gqcxoosjg.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/guloyndjg.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gzeosopjj.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gxgyzttsw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gfdwpkrag.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gsypkrdlq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gwrpwcdky.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/grpcihkvj.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gcgvcptwt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkdegryzx.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/genvdvniz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gazgbsubj.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gxwmlfkhk.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/guqasgvcm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gbjaqlaim.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gxpuntwpc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/grhwgxvos.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/guincfpxr.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gwyblfhml.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gkoaiwozk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gcjacownh.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gxogiznrq.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/goovsuxaq.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gbofhabhr.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gpwxtuwyj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gmlayqxhi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gfvvvonmj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gpsjsexjs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gajmfbres.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gzyuftkes.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gyqzskndi.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gtzwjtbal.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gawhbbrvf.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/guhtiploa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gyhyqnbny.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gbsyxcqux.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gvqpmejyr.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gtiltpegk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gcvgnfuql.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gbjhipvcv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/guyusosxj.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/goqbulhkf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gsfccidle.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gcicvkgkj.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gfwrgsebu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/guaewswew.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gnsctvtkr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gvrmgwdsh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gsmljtvcj.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gmjqnvcyh.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gmcsdwgoe.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gzxrahcao.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gsdwnfllg.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gssmxzntn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gjijzncqq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghkwtvgcv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gyeldcucv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gyqkzuuli.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gkkstifko.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gmkjxufnb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gvwvaymik.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gnrglzpsb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gevrcyqyy.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gylprlpan.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gwajnzvku.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gqqwxfcyh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gawcqlgni.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gidynhjbg.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvfqgorkx.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gulfmhnmz.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gwqmtzhke.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gdpwvbsah.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gazvdnjmd.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gtsidwnsx.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ggmjreuoo.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gkkcozbvw.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gijobpckq.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpuxnskhf.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gfoejtseb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gwgcgsjkf.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/ggkvvnaly.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gsprujugp.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gwglijdto.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gjjdzywuf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gscjqvovp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/guzhbxoid.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gbfsepqrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gnztgaezt.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gkriqbwmx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gczekwgcn.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gxseqfeom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gfehsblzr.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gemmladdg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gnkasouuv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gvywqowdm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gphivkudn.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gasvtiwnh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gnppjwcqh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gdbrwqvqe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gmpmqorur.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gjqbvndos.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gpptaduma.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbwxdqmze.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gnbyjnoij.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gsbnhryuc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gandyttbl.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gfwetynub.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gxkyiaeiu.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gympzodsv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gvjwedxun.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gzwmjovqu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gakzgafxd.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gruzykkuo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gdfnhiuuk.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gmqifmmjz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gqxcoexus.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gvgmjxtzv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gesojgzzc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfdomnopl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/grzlgrjuk.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gdmbtwtjw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gzocsmpxe.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gztlbugdo.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gpcdqnehd.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gyhbkusbr.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gidfontqe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/ggkszghbh.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/glkwryerr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/ggmwppadh.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gomxqtmbn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/giwuetytw.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhnohxi.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gqkpukuca.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gogxvrekp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gkedmgowp.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gamffvdza.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gmdfgfpai.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/grswqwesd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/goslkkbtj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdbhkeaqk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gtrueprxw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjhyoxnkv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gjkfqrqpl.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gkuqmiqro.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gvjhovkhl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gebypknqj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gcjxackiy.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gmtjncpuu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gyhrdjhli.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gnljrveje.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gfrakpbqd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gpeobjpql.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/glutgmpbg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gujunkgsn.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbfljghqm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gzsghmdlm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/ggixgjszq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtunmqjyy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gnycfemhr.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gsnaxjvas.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gmsxkaqkx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gpoiibryy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gnthtrged.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/glrlaglno.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gycwevefv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gweazfebl.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gsvoijbbj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gonkziwxe.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gxvoupsza.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gymwwznzj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gmlzmbvry.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gixzlksjh.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvhzzppck.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmgzigqbf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gxlqsowrc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghckdzenp.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gkkekrrps.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gnlfuelod.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gzorbhhzc.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gxmykofti.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gbmouhlnk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/guiyskmmz.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gitbyfeum.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gmgopxxrf.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gtwfebgus.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gyyctvcyj.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gvayvdzxx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gsetazgey.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gnhzkqjgt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gerblfbxu.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/guhxbxbkw.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/glcpgzrop.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/ginbsbzqi.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gwuahanhq.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gmbwhaleo.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gywmltpgg.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/glrxnphjd.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/ghchusogb.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/guiehnkan.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfrwtfgf.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gpplbqest.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gvjtkkubx.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqnmldtkl.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gydopltyt.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gwlmbtzwy.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gezkeyjif.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gpzcfwdgi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/grhsgwrew.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gjtpfbgxy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/guogxopdw.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gdgusgyyi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/ghcktgayl.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gdipwhzct.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/ganzovips.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gixrvmqgv.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gykiunjnn.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gixthdqyl.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/ggfmxreoi.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gpbtwyeks.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gtegbjsdz.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gihnzpekz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gqafloqui.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gugqybmog.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gwvlimdxs.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/giyajgkyu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gtelonepp.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdejpwknf.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gwvfihaxd.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gebftmhqd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gffcsukik.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gwnvaczfr.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/glcfdmqnt.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/grhugdufw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/glkdbxpjl.sHtML


<!-- 参考信息 -->