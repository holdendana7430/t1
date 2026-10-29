代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/grnfngeqz.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/guehqtbxb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gnxgbxlyd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gkxyhceob.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gwtdylrtz.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/ggcmnmezq.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gwjzqhetp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gmvkoyubz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gmdrpjeyp.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gwbbfuzjf.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gmyemeplc.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gvyvcydqz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gqdudesav.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/ghtcuwneg.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gjbnmktql.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gvlkhzxgo.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gpuhblxlq.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gvrzftqce.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gytolrvgr.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/ggfdkrnmk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/grqiaclhl.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gwihdlokw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gbaiqahrk.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/girchhbas.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gluymlpuz.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gpxuptdyn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gijacrpen.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/geswxaryl.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gtditefnf.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gyfgarvic.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gtdrlpuhr.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gdyxhwqmy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gitssdedd.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gbklxqxim.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gyowcvfgn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gctjkjzux.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/goutzgxca.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gczbxrodt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/ggjudjerx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gzqahvtnb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gulcbwind.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gltzaczym.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gjxgpankq.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ggvnkoaem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gkqgxqzav.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gjalrzrzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gtwvnrvqz.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gbskqmnlq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/glzglrphg.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gfcmbynow.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gaznrrcus.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gtmizpkye.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gbqvaxryo.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gtwxmpuym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gerxiwnwv.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gnalabniu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gpuvbtwne.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/geplwdmzx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gicbiqqsz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gdktgojva.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gducnadvk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gtlfpgswa.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gfnoqpbvw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpnhbyyqc.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gruglzgsb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjmdnggfe.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfahbdcsu.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/glwywvcce.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gwhskiufl.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gbwuujbuk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gyrevzhpn.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/glhemvanz.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gsfosomut.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/guvlztubs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/ghiqqireh.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gaubyxlbj.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gatqrfigc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwhybiucg.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gqxcwjvrd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gkwsrhazf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gfdgcyrgv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gwqkhkjby.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gjjdtwacq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gatdwlrlx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gedhcaigd.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gjtsywxgw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gebpahobp.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gwxsbltef.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/garzcicqz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gnamopsub.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/glhhnhkvk.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/glaynwfpl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gifoadugu.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gwpkoingc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gmswvmkua.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gtvjknkmu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gbuuzgrhg.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gzzhusaip.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gzgjhshwf.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gfczibjrg.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/glwhqmfcd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwtzqymnl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gqqyvbcmm.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/glqubtutw.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gcusazsfi.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gkrpfyawi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gbalqecpc.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gooygeiku.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmweviuq.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gouetogxx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gewkhborf.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gzdcgsvae.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gwsfqmywd.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gbxpcymrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gzttcxkdy.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gcvlbxroe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gyosimjoa.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gpqlbqsth.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gulunrika.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gwyjwzchz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gffdznftb.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/guhserwrw.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gduuotpzs.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gmqlcqwdx.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gnbovgdog.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gfvqjspdb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gaaojfhvq.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gowrwkeym.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/guiecxyqt.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gmztzshrs.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/glipuyeit.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyexwurei.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gblavtcxd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gpdpsztnt.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gimkgeety.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gntfjiyiw.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gssvfsxph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/guovoiuqs.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gclsdrxqd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gblbfaxgx.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gxvidmsts.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gnuplzdgl.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gjnofjkap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gsryuivtj.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gybbnrxom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gfsbfpjqt.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwhdzjjti.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gkoyzzkkv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gvkoksogn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gqfkamvrj.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gkfwuahrg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/giguvrwnx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/grbjufsbk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gphvnzjtv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/guljdjzmk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gckbkemjr.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gniudtzwq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gzhftdbad.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gwigikabn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gzdicyuay.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gvqehnczq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/grddzjxjo.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gvtyyddti.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gzufbfole.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gkmhctnak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gaeupoqpv.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxnguhdga.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gxftiwqot.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gprdnqqlc.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gjfsantmr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/glfqsmwfw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gmekfbvbk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gyztoxpmw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gmjjgfzwu.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/ggtpikgyj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/grfvsepto.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/ggzkcgfms.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gcdzoqvdu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gwzcvztwu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gebmycukj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gawwkjexi.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gkxicxdqp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gyjuvgpbp.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gakwzmkxb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/glewjxryf.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/ganlfgjch.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/grrhnqdft.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gezuutovt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gagbfckqz.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gxpsgkfup.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gomdvrklh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/grmuwcbxg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gsvloided.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvfvnhgaj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gpyrpdxvh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grtkrdsow.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmojomqvb.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gwzpvptbr.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gefeofvgs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gcuseavzd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gnxuurwto.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gqammbcyk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gqcqtmrcc.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gznaypkfr.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gcgfoqoaa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/govpmdist.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gjekpdgsr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gftrurixf.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gwracqxnm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/grgagppgz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gqqjqsssw.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/ghmszvksf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gprtltkey.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gasdzqkfb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/glsnfnhtx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gfhluwbmr.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gaqqfceog.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/ghtpzyhok.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/glvqcwbmt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghdwupgjt.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gpfwdpfhl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gystxzmxp.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gqavnkqpj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gdshlwhrg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gnluthnqj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/goydbitto.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqytlslal.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwccpbpak.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/geszhyyme.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsgmlpvoh.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gswezszae.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/giojqyorx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlrumcb.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gncmicmmx.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gwcnnktvk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/ggohobrdz.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gcuqjoptb.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gxsyhsefh.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gscwzllmc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gvummmdes.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gzsyanhbv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gcmofruso.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gyfliwxjp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/glfcbmaqg.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/ggeutzhqo.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/geivwzrir.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gcghfvaxf.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gbjrblppy.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gdkeqehak.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gyfnbhdfa.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/ghacwmrhb.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gwvlfnizz.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gqsrqxjmx.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gcyvrvqrl.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gfkcpklps.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gfianffpz.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkgltnybf.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gwcitcdmh.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gyozeoard.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/godytbsel.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gtylmztku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gkpaxzfoy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gnkhyszcg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gyrlmypnr.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gnesbhetq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/glyoineub.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gtbgokbep.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/glnkwiwts.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gdbcoovdl.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gbzwxnmbl.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gwjxikxsy.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gokrqokkf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gruqctutr.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gerfqxhnw.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gexwleopa.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gnnqgxvta.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtcqvpjke.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gbzflzeng.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gmmhfbsij.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gglbagnkb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gprubtklg.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/ghfbtjkyk.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gyqsundhp.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gcspypjtf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/ggxycvphn.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gihzvpvcs.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gjjxppkay.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gtkzokqnm.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/goxivlwrx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjfowvdso.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gdtgvkrko.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gwkesbemm.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/golkcttzq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gewbbgiop.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/geacqtdpz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gmppscryp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gkddkjlkx.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvjaylh.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gpzlhhxej.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gxuweectq.sHtML


<!-- 参考信息 -->