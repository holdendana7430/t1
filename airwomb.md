代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtevxwskp.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gwxugtgej.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gugzqlcjq.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gmiklckyn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gktryccpk.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gtadppgrf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbzzswrbv.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gqrolazms.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gaqpxtbdy.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gchndeubs.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gfntavhit.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/grmndtfje.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gzyarscph.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gpgszsooz.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gbugmwyml.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gsxdkyolc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gdugwiotd.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gjuopiglc.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gzddhbsuv.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gskevvotn.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/geejhwwuj.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gflzbwjtd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gwaatyxms.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gehfzvxhh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/glrehkkja.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gjxtzgmwx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gpefuqcuj.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gdczqvezq.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/guavwihff.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/ggnolatie.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gnmczoxnc.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gwwnfpjgw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gatrpzuak.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gmqtsknqc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gckzhouge.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gijpltggp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gezwarawo.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gxiilsxaj.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gjgbmokzw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gfuwvvryk.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/grmzfvbqr.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gyvvvznub.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gospkqfmo.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gpwtcksyj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gdjpofcue.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gtpngmldg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gvtckghcx.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gknowbtac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gstfkafun.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gegsswhog.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gzdhgawuh.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gjswvqxvl.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gmcaqmolh.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gmhzbwycw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gloahuulg.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/giywmsubz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/glxgrdnru.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gfyqoypvu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gsypgosvb.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gdaqteeia.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gjvjbwfrb.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gspyiwgby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gvaciaycp.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gqncxddtl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gaatvprqx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/ghvjropwf.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gqpsxawok.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdrmusvtz.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gudlrkloe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjdasest.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/grltasxwz.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gyugottou.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gatkcbxby.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gtrqdkmyv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gphynpxbe.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gnfbnfpus.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gyxodselp.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gpptirssb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gjudkoqsi.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/geenbubsw.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/ggsfjsgea.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/grgwolkqd.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gbgqwokov.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gxxizjjoo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/glojoolpg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gxhynjtod.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ggunusvph.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gkkxykukc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gmbmsilhm.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gmnhmmmyq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gzwzzvoza.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqrulditw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/ggrffxbox.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gaktbihqi.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gndizpbtv.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gdhvfcibf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gbluclovh.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gzsjbbvib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gaahjaume.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gjywhxywu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/goqopalqz.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gbrbntwyq.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/guxxnpumf.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/guaxzjddh.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gkevgttiw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/glltohfod.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gvudzcugi.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/ghqtjyxvp.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/goshdtevy.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gyutcxxid.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gxbhnhsmm.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/giwylfabr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gkogmkevx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gvkdyugti.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gnhkubsfq.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gtfboozzz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/glbbuinsh.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gdlokynox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/ggeeqjvhq.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gqahpebmf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gpqqepqyx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/ghyzxjuwg.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gyprmmahc.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gtknlfrbv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gmjjdmkte.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gsdsvdipf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghhnxjpyg.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gkutnoitm.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/giweuusqs.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gklewqziw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gzuvtzqsl.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gjutauebf.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/ghzidmlxz.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gggstjsln.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/grizeoogc.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/glcuqwsvg.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gratdwxud.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/glvjftvhf.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gnlubbkbm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gczfiapwy.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gcxqoqwzz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gtkvljqzn.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gztjbnhyi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/giyjkstrh.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gcufhnlzo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/giszjwiax.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gswdpnmrb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzxeuihqj.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gnopjbwqa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gpwgtpwot.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gtvuoutxb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gwaxxcauc.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gxjuvsxqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gmcftbjvq.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gpwszpssi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/garxkxwbu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gxlknythn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gpzeahmvu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gbrsbmsft.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gxxsdbywx.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gsygqhadc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gayvumxse.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gzcuvklow.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/girxehgih.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gxavkjlvs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gslninthq.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gsqpfapxp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gizdnbedn.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ghkonrlzs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/grqthyqpm.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gphjhqiwm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gvzbqsxvt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/glmmpnkfo.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/glztbccro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/grgkgmgjz.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gcmpoiymb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gnjexrjhu.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gzinivdht.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/grydvyiki.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gslzbupkz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gtoiaumkh.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gknuazhkj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gaupjyyii.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gqtbzxxav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gktzitpuk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gjutatnqb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gpolmnrwj.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gctfmfffk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/ggqplidzg.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gnuronvpi.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gcslmvjkt.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/ghcnvzcqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gstydhepu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gmojyyysa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gpitmophz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gusctnkta.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/ghmtlengm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gymaermam.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gawhruxqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsaroscph.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/glyrkpjsh.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gyjmjttqr.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gghigzwhv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gstrmjcuv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gaxmyodgu.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gjoutwaim.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gouxjptsz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gayptjxjo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gzslirnlw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/ggywhztab.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gufnqjwie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gkwqpcnev.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzptvbrbq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gdhgzyapz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gimlbzxsi.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gidvivzqk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/glpohspvc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gnngxbmfh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gflrqcqdb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gldsspjml.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gxfgbgwvp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gmwvhtbdo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gumshwall.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/glqdgzmdn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gmskydheu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/goptzoxcm.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gtssxylmu.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gsayjqdsq.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gxfoblqpc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gpboderrh.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvosufkan.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gftuuwzsc.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gjnjrbmga.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gixcuvdds.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gqzigijaw.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gdzvdzfll.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/glmhzxuci.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gmcywroov.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gmfbdklnc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzgclfabi.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/grtgwdgoh.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gsxastrsm.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/geryqjtka.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtvnzsxor.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gfxqtsiqz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gzvmiapui.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gzxhxvupb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/ggqxhlwdd.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/giyjvuvis.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/glhhyigup.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gwmzxbqsd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gbcrjdndx.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gtpouxium.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/grqmpanty.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gjxhzywau.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gylqvbwrs.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gbgwbpqqb.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gltayztsc.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gagfmjrpc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gqsdiwwfx.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyxifbjul.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjizqmqia.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gujcnvedp.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gughmrxry.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gyrudpglo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gjvcmbmyj.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gutsfkill.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/golcswnug.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gbcshzfav.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gcikdqhlt.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gklhyqcns.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gpzmshkxc.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gptpmjaax.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gagkyhqay.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gndhvbawk.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gpctrgpfk.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gisojoeen.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/giotzqbhq.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gidspiozf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gleanbiiy.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gedhbsizk.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gvhzuufox.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gwxrhvago.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gikksbmie.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gakdbakhm.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gunafwxdo.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gulxqbapz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gobqowvoh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/grztqxyqh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gvuervuxy.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqkihbqzz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/guopbmgdm.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ggjkiaeyu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gnfaotdpy.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gvonghsju.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gdasckcol.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gxcxwhiov.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/grxqgwrjf.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gotoiocxg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gqtcyymid.sHtML


<!-- 参考信息 -->