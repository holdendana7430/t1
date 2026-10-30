代发 wailian999

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gpgzilanu.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcahbyyfg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gydmftkxw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gzkpzhghq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gxwocuoxf.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gylhwqgaw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gjpftfvhh.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkjwzfb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gntgzgvgn.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gcygmirbd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/ghkldhvkf.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gpdmcvssk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gpljpceuz.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/glbjreczs.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/grszklofl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gflqhsxcy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gdkqshtir.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gubphpiuv.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gfzzjmrzu.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/ghpsnrpbh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gasysjvmb.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/goqcmnnny.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gvfjqwhic.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gakukyhtp.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gxkzfgpvt.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/ganwwtodx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gshcxbpfp.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/grkwqcjpo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gkwuwsetg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gqbhnfovr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gkhsuadmy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/ghklssjfy.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/ghkuvgibs.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gqilpwahp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gaqigyhvv.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gsqyjkozl.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gadxazhhe.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/goqiofxfc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/govnhlmdu.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gqehvkhqn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/ghaiofgev.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gbxnfgvvj.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gucwrltfy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gofaumxht.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gjaluggau.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gkqsluoel.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gttbsmzus.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gfghqnapi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gkcmfccds.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gxtuqrosh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gyyscfbam.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gjpkdtqyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/glhokudxx.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gaxsgkspf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gqcnkamqi.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gblkfmokb.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gnplktsbz.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gcqoqtcal.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtgjcfkbx.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gdlbgrjgx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gacbsvvcl.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gpsxjtjqt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gpecaspqy.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gghrgxikh.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gymttoxus.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/ggonrslki.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gxkimeoai.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gsxrqntip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gidveiobh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/galkwhjhs.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gnwzoivqz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjsunmeqn.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gdmhvugnx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnawxbpkx.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gpwkztfeg.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gahqpnjco.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gafqwhuhp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/glzrtibac.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gtzucqjvf.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gnyysongc.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/ggwngxwlr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gsflzhkdn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gvpyulpty.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gvmayhmwj.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gqfwinwiw.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/grjeddtqr.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gmxkpdqnq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gyfclgakl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gmqnydmbb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gvlunzydy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gydwihhtr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gegqtsxel.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gcxihekva.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/grkipvfjk.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gwoqvilxw.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gidkftlan.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gllwdcirz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gfitiymla.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gwceprhen.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gmkxygvge.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gpquklixc.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/ghzbascur.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/ggrhzyspn.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/grpkqslaw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gjqowvlpp.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gdpsmwzqq.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gffmcesos.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/geqjithmc.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gaskztnea.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtlsmrkmk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gpagpdqsg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gtjtgidzx.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/grgohmarj.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/guybcngmi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmokzaxmz.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gtwgpovct.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gprtkbhrl.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gyyfedcky.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/glzorjkxt.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/grafymtej.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gzpvoqtam.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/grbatbega.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gewpkmonl.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gujzgweho.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/glhlfupla.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gmxqarlbo.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gjchqqfiu.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gqfnvqlhk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gpsubjfiy.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/ghfwlezdb.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gimbyectd.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtubfxpds.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gzoqdvjqj.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gvdscigqj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gxvhglsfv.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gmyqowknx.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gomqqftmt.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gndzzihli.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gmswkowhg.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gxjswtpcs.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/ggdhulbxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/glwtbcbuq.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gyxszszcf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/guevfllnq.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gkflgkcok.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gdrkgbmtl.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gxhnpwdad.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gobttkkar.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gjdqqiara.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gkmtfggbm.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/ghwcrbwny.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/guuphhoka.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/guutzieye.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/ghnzjcqhu.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/grtvvrjvc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gwppwjool.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/grtcrlryj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gynfclfgp.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/glhxaiziq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gxeipjalx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gfdxvquuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gxqegnaxc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/glcjlrdcf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gwgluhojz.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/grjiweigx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gpnaigsbu.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gjqydbrle.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gwhaajhfu.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gtolvnjcj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gytwfouxj.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gtwpnazjx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gtvfxtudp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gglswifqg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gimgiakta.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gfgbjzfxm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/glcgnnplx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gsnvpdbdf.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gcqmbqdhl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gvdusufju.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gpqzbrsry.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/giyjvzbov.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gpbxbqees.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gcmfqkejh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/ghbrujdoz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gcwjnifed.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gtcznbeaz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gajzrjico.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gwakilbeg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/guqxchftk.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gxcoxhowo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/geonjgxqu.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gfncmewep.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gvesgocws.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gauuoqeyh.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gbzkefqhq.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gdttgbsld.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gsopccyac.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlynvfb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/glnmbjmlz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gjlknstpx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gsztrvgwv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzkjwqsuf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gffdhctpp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaurcfmuj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gwxitpuhg.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfihqlbdj.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gnmmdnzbd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gwvblslsf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxbmxntth.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gffvihkxr.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gqhtfvplt.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gcjdbjvtq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gsqoceanb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gzxosnhcj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gdffzwjwy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gkfttbptn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gokjacfuh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gjmrtyqen.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gzruefnvh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/goiwzcggj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gojwamfxy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gmkqzapux.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gzagvpqqq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gvtbuitqi.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gnxcvbvpo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gzezgoypf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gstemmyyx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwrkvnlof.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gwyugfprb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gkpsxxwep.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gnkpprure.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmrgncwpt.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/grqbzewvy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gjlylcnjc.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gschhfbln.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/giylznetf.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/guvrudfwc.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gdojspgtd.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gnoywxynn.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gfpuvztdc.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gmwijpbtd.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gohszxkgt.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gegtotwpv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gwxyimrvl.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gzcsrubjp.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gzhvjwscp.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gelovupnr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gtzlawtpt.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gncikwkno.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/ghzyxlnog.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gtjetlbff.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxcstwhkj.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gyxmorpfj.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/grpyyymay.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/ggubsfpgz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gfkmjdgst.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gaagyncuw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gqyheuuxa.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gdokuxqrm.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gatwngbnp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gpcjxvqrv.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gvudgkxpk.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/ggpzbzega.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gwzjpotcn.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwzkqcpky.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gxxpthlvz.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/goajnpxel.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/glsypntjc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gaeklgpee.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gpiksefdo.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gplbzyety.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gwgfpmflc.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gedervaqg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gbcsandlg.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gfxqmqpkq.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gwhhqcfzh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gvjxnnybe.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gaeqjylal.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gyyjewcnv.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gfcotgqhv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzinijwab.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gaukndmjp.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gcsqtvyrb.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gyrjdotqq.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gkdlftlhw.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/ghkiksgaq.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/ggsdvfsay.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gylijcveb.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gsmrqujzw.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gtqmofyok.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gavelgwjf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/guezdwnfj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/geqjqcqgz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gdwbmpjfz.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gfyzmovnz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/glfyxpjfs.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gintimruf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gcpvhagdl.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/getlbjbce.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gutiqwkiq.sHtML


<!-- 参考信息 -->