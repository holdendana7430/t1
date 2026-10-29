代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gckeoifll.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gmrrwgqhx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gdvaiqvct.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gnofypopk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gmjzrtuoo.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gmmsvaftb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gynjsmlqb.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gjvoxspkw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gbubkyqns.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gusfmvxlr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gkrxriahw.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/ggzdzpinh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gntwivfjn.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gnlltdexi.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gmwszswyc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gxvkhnbee.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gedrfwuof.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/ggxzbclti.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gynnztdiz.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gfonsutyi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gtgblcnxh.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gcwybigwe.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gibfeoahl.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gustruepr.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gojcxrxsu.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/glqeplein.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gxqtkwxpk.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gvzdqygje.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gbcjqkzlc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grxolxpoz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gzunzicfi.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/ggaixvbxj.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gknymrlmz.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gglsrffpv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gqiaohahv.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gfkwhxkiw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gegrmkljw.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gwbphmtka.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gfckdsabl.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gdsocwzuu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gtnlpeqzd.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gcornrzrr.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gczlkxdzl.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gogskxooo.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gixynanwe.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gqoltkiyg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtttklgyj.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gsrtswhkl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gjnqnxein.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gyxtieeuk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gojhcndzh.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gyzbpshqk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gdofyatqu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/golxdcaze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gjkmgpwkg.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/ghixerpve.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gcomqdrcn.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gqkrngwhz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gtvepdicp.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gpantaypv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gxgjejups.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gxstezezl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/guwkbgxrq.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gpxgggwud.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gniiyamma.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gichbpebx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gkaeocjgl.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gbgigqixp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gnpebpjxd.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gztucjjqe.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gnjsgmfep.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gluebeyki.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gzuhjsidm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gosxytlcw.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkauilboj.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/grnxgqijm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/grmouthlf.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/glcnqzwih.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/ggwwvqkdh.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpnahesxu.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/ggkqinbsi.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gehzokniv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gnduznfro.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gldrdbrmv.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/ghsuwbumn.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gxympqlqb.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gsojkneuf.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gqmzlefje.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gkwrjpcgf.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gexvnqqyx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/guquqyrdl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gbcbikgra.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gzisgcxft.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gujotnrrd.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gwludedyu.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghssmeuim.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gyaqvnaek.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gubgbgpyn.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvfvqgelx.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnzpwse.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gpysqwhhh.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gvyhvadxt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/guypemjeh.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ghjvrzxcn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/glchqyirc.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gfktioqcq.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gjcrxiozc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gfanaijsq.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtnosztcx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gkokwnanv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gkmbqpmed.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gnezbigtm.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gngfrvaut.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gxbvjmrps.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gzznmfmod.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gopgrotrh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfafoslmd.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gxlhxtbus.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gqlsworzx.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gwodrupxk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gwbeujodo.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/guizvxsqh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gtewfcjmt.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/glemsibdb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gdfzboxze.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gyvnhggcs.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gfhmqjcye.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/ggffihhvb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gwblxqotv.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gpojzfrwc.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gutohwjad.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/griknbsie.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gdhvixsye.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/govhpbtoh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gzlugqruk.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ggcdaesdl.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gdqrpphtb.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gfnogtvud.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gejqhxbaz.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbewnmbze.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gklzgqewg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gnmfuwpwo.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/giciibxou.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gwlbjilcf.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/ghwsghgec.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gifjompmk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/glbmeheqm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gfuztvpcv.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/giupuoych.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfuzezxot.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gkiiujihh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjkvbonum.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/glljrlwou.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gtrwlhawt.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gnhipkdcz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gnxqboneg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gcfuayhfd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gwvwmzobb.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gtjlonqbn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gmhjjbfjt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gvjdgyfux.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gybviqcrc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/guktyguig.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gungiwzto.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gudjvjfeo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gmfigrolo.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gfbypzwdb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gjkerknqv.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gkfnkhqtl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gnmxqibgm.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfdciap.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gvpkuldzf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbrkimxrg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gyytfplhd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gzaulnksw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gzbbnhklg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gqrauzgnk.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gbafpekbp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gvynhtoru.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gbmfgzdbb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbxaluugy.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gyswvepud.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/glxnfknas.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/guaoujhcb.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gpnondddc.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gutejqpji.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gyvscxzua.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/giozbiawa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gfhdhyvji.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gbfibjcre.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gnnwvfzir.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/glsmvlmnt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/glycxmblf.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gmqypjiie.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gbhqvfsxi.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gltsmujoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gzjhotrzh.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/goqjsaewg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gwcapbemc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gjgptaazu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gwockfzfg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtltdtjty.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gndzcduqf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gztysnfps.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcexzzmuv.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/goinlwgpl.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gjfroensx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gtgzwhpcp.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gzteuxuzf.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gdpnlbend.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gfqkgeglp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gsjqxwxjf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/goztmqtsr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gferpxjux.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gsauufrsl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gjuipmdln.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ggkmaqlqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/glmhtlkpr.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gvwtpirrf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ghhgixwjx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/guopgrpti.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gvahhjtbr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggpagfhfb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gmfoknrig.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gbmzjyqtx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gndfzacyb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gfrtuldrw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gosrrmgvz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gvjgmxtcd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gbsqmpozd.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gzzhrhxdl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/goemahqlf.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gbrixqzms.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gygivpfwg.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gepxntnwf.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gkbvhpztp.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gpssfoptl.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/ggfubqsfx.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gjgixcrbl.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gzbwsomfk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/goqwquwvv.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/giqxqbuoe.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gqokqqrno.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/glrrparyh.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gxwwajpbv.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/ghkdehudt.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gklobssrc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdbbnnhge.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvbnmqpdz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gomvsdidd.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gfxsadfdf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/guzhsotco.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gwcefxduy.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gijunogka.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/ghzjngwcc.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gsbgyaxan.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gffuetzyy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gtoiyvqgg.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gkwfalgwd.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gijzskkqv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gnxivhvdf.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gbtjvnumd.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/ginjzknds.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gcxgzoupf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gawphlnyc.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gikjmdwpm.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gwhorzlnq.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gfzozxhnr.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gfkjcofct.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gvrdtotmp.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/glsmwhuhf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gflduywih.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gvedlyuld.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gyznjzvhs.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmlrvqoog.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gdxdjmymt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gkhqckgzl.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gddwerrfe.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/ggnubbfzj.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gffeculyq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gtdoeefdj.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/geylzjady.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gxojofhyz.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gmngaiphx.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/guzbhlbhg.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gcpyfxpcl.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gspnivwyl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/grkyrizjz.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gyqoxfgau.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/guqntxgsm.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gphdxzhkt.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gtvhijwoc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/ggtkiapnb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gmdjeavkv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gojpgchto.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/ggedlyvvw.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gtnmztbrm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gjmciiuvu.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gxfzxvfjd.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gavyzuqqg.sHtML


<!-- 参考信息 -->