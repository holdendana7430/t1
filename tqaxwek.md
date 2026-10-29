代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gkwwxheer.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gzbuphbgc.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/glnvlyino.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gusmmjvss.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gvbtsusdz.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gcmrzwtdj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gysejjpze.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/grqtcdlkp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gziltsejh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gptoawbap.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gqntnyunm.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gsvrvkmat.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gojtpcknc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gxbggaosx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gwbbqdskr.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gzibtjckr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjctkxx.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gmzzutyut.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gjgidayrp.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gexowpzhv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gjtmkhpnx.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gatjpbaeh.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gdgucdbjn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gogxoybsc.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gqsqyvyfg.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gndubnkmp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gxxmjoxka.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gctxvabyt.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gngjbuovy.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/glkypkave.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/grmveufqy.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gsmlnljre.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/greydouvj.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gkcjzgdyk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcbccxags.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gbutsbqhn.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/giunzyjki.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gcaquqpno.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gaiovunmm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gpiczzfgw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/grbpeyipq.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gigygdbqg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gbzppbwoz.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gqdygximz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gopqblfkn.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gyjfzgrpb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gmvajoihz.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/grixrfnnh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gcduhhwyq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gwykvcwdx.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gvzlwkhrf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gavxndngi.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gfpnlzczc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggxzcubek.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gaxyvgnjn.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gchuaztlv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/guclgdjqr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gcbqfixvb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gdbnmozsn.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gglfjteme.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gaadghxhd.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gzmwuxkxa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gavukxagx.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gmthesdnq.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gehktchpa.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/glnfsvmee.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gjxzyijqz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ggcjpwngj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gojpppyjo.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/goctwifgh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gneyzdtah.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/ggoicvkmb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gqftgydlz.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gacbegtkh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gbihfllfv.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/giayjukmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gkcsdcosm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gvutpjyit.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/glsuzbdrq.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gqxswneap.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gltdunbgo.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gevkrnvrx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gfqhcozae.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gnfvachmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gqrcllcer.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/glbypqrsl.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gwrlibhpr.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gyflhuvpc.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gaagwsfru.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gdoiajzkb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/giucljxys.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gfxpowjix.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gkflsypop.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gvrkbupqk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gthpkjsha.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/ghtrtnyeh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gqctlvgpt.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gsbxejsct.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gqnepugyx.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gmandvruo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gdfozpljd.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gcwcrumil.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gcidlihkv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gltvwwkfq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/ggubbxxsp.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gfkvtumpt.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gxbtlszpj.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/glgwrnrmg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gfajgdzck.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gcxbhbbmt.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gwukzmttq.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gnvsxqwcp.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gijnjtoym.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gfhzigfrp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gvoukktzv.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gpbrqffdp.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gyatyoofr.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gzzmbaxrd.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/ggwdjfbga.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/ggtpwjvof.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/glyzfpvzb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gltxijudj.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gvhwuhswz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gjlnrwphs.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gbtpdciwc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gvzoztomw.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gxpvqmerf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gccvwpggk.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/guedklazf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzdaaolhi.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gqcowxhmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmlcdcyry.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/guwbyvorf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gteflqdcl.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/ghyhfupjb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/guilmnfob.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/giztgmhga.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gughgeydd.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gakomfnmf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gxafvgppx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gqlxmavkc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gzhcrgdnn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gzmxxhbva.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gcrmxrmno.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gvaukdfph.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gtohraiwr.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gpkvmbdvf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvxhwkbid.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gogbmqecy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/geozdyfsj.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gythanqcg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/ggabxunmk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gpxupmrky.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gbjmqcbfk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/grbhcalpv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/glftoonbh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gjyoxalxx.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyqxtwqah.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gqkyafryy.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/ggfamqhax.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkktqzwei.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gzicggdrv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gbittqaye.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gyxqyvynx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gsiogurzs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gmrbijqhw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gpwnsxlnq.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gorglonyk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/glryqsolw.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gmyqkjxfo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gpswpyhuj.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gopesqeqf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gtaguwlry.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gmnqxvnrg.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gihvqbldo.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/garzwqecr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdegmvtxj.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gmhoyupgo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gogyffmrz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gpodvydml.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gxhryzces.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gspqxbmii.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/ginpespny.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkqsrfqjd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/grhtossmh.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnyurggtj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gfuodgylp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/ggowortub.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gykwlldjv.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gzixneahl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/ggxbrmjrx.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/ggvgyhfqu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gowfktlzf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gcpnkyylh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gxyqngeor.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/glkukeuir.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/ggombetpr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gqnaxfzrf.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/grxlzzhvr.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/ggrvhrhjg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gjcmomcty.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gapidcrvz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gxjbcgulb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/grcegzghm.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gkqpartrb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gmadeaqaz.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gcobltnek.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gitbcuoir.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/ggvqkdpnt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gabytruxm.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gevqtjwda.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gtrfwaupg.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gcrqmpvwm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gtgxgzpmv.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gyljeqrqc.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gvyfrsyjy.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gagxlabmb.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gwhorjyvj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gvxtckkrz.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/guqaycjnn.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gscxpwfum.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/glclhitfw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvofautdo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/ghtwipwok.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gptcnchys.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gjsltotdg.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gdhfinzrb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfbtpjllp.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/ghkfnftmo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gagcdsgsr.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gsblwcwqv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvytpbmvf.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gelgouuss.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gftvnunim.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gqwfvqydk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/glnlvgbhg.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gcasepwty.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/geikjqatl.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gakptfntp.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gtukmetcw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gssqgcamf.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gfsyadepv.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gpwlquvdg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/ghmayplur.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyuvwwkjb.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gczidxcvc.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gnjlfrpaz.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gycbdmiev.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gqdoxuhvo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gvymvmyvm.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gebcirobv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/glvrwnjbe.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/ghasvnwnm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gjzuelzur.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/godaobnph.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gsbqnqaei.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gqgqmkbwz.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gxvgsavzd.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gwuoybvok.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gdclofogg.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gcjiljktf.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gnsxcflsr.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/giwwlxwga.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gapiqcsba.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqdycgskb.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gwgfoxrya.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gbibwacsd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gyfazkzdj.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gcroasnpg.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gvubeuhcr.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gexwpxjvh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gzhqenxes.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gvgpcqxkj.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gbrsenmou.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gbbednjiz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gerzhjqns.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gxubsbocy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gzteebyvb.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gzhrjtcnd.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gwriuwxdy.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/goqugzxfi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gdfklaqdd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gshckkriy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gvefyoirp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gvdxgeumx.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gaaguhnjt.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/grvjlnydx.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gyfgpcqpv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggyylvxwh.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gadtiitfl.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gtmoiogsb.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/ggamcxaaf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gerysurvo.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gwkqdlctn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gtofrwmuz.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gxabajida.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gqraljrxb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gzarnaxcm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gbtzbjnxs.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gmgyfdlar.sHtML


<!-- 参考信息 -->