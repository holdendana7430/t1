代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gyfrpjgdp.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gofruikwa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/guxkegmxi.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gkoudafrq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gebyzizue.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gpwcoomiz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gpllxqycr.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/ggfntrxaz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gvzgkutnm.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gttfxbwsz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gdeefgdoa.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/ghawbbxvs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/ghimjgcwx.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gqqlfzuuc.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gzdsxrrzf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/grjorgrvt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/grcjmeajc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gbfvlibrg.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gkrnzluif.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/ggscnzwrf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gdodibpvw.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/goztkrqql.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gxyybszmj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gkhjorryl.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gwwphqhmq.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/grrovqdev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gxjkxrvyk.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gtbxdlpun.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/goarctntt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gglrlnyex.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gcmhxlyxe.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/ggnvmttqw.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gszprlqpz.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gakdswrzo.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gjodvjebu.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gpgigxkbp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gfpwkllyw.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gusedygum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gaiisgede.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gvipclzkp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/goisoatkd.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/guzuioitg.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gjtfcvphz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gohjlbasx.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gjcjoantg.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gtvhijvna.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsiwihjul.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gtldjivsv.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gpkpejlrj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gusmjdjyp.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gwpaqydxt.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gpwdtdirk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gfkslgdei.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gqrvakpes.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/grolmyzwx.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gematkayp.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gjidrgtlf.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/grrqmtxbg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpwtlfa.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/glpelomlc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gzqvpecfg.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gnkagvbij.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gaobaoaip.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gqokswiwz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gszfyrrgd.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gyukvgfdb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/glmazjiea.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gsypnwsup.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gxmdnubhs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/grfxjncug.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gvpuboujl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gulfpypeo.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gldflssma.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyhyhgcsx.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjevquuaj.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gxbjmxpqc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/greguaumg.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/guphdbyoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gmvgpdknl.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gsehczcfn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gfoegtogg.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gypmnyrhx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gqlozfmjp.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gavnokqkl.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gllqhpwdr.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gdvlihlbe.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gbfwktlkb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gwfhlaxci.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gcpicjuxy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gkbpyayan.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gslqmhqhp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gytgmpduf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gvxuwfhcl.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gbuqgygwe.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/ggrliwtgm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkkglocdd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/geymtkerj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/giqgusieg.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gbkbilvoi.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/grocmcfdi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gacbmfcyg.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gcicwkpty.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gjccgwjpo.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gjkktoyqb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gblgjruho.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gvbsrichb.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gqgaxzzof.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gefowonas.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gzgrxkhau.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gquigkmld.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gdvqealiv.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gihwhyikp.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gswzdibvh.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gxhqcdfyy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gbwjebqii.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gijpojjay.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gtdkgdpbz.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/ggylrxxyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gnwpyvvoz.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gvxteveon.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/guqemmevl.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gvcisucmw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gjcldoeep.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gespvxzmm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gziswbwjh.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gvzfubfpx.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/ghqsstsix.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gajafvcty.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gppcfapeh.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gvzvrxroz.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gafcmierq.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/goxsfiool.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gehjhvvim.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/glckokihw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gliuhsjgx.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gapxtmofj.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gxiqbexmd.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gqtcxeuvd.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gyebaxtbm.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggdktojev.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/grguswyut.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gdgawmvms.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gpiqrqgfo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gupcplvro.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gnezzpqnn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcyayfefl.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/grhpdlkox.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gfgdwaqcf.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gflgdtkjf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcduzgmpt.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gmetmkisr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzbsqwzsd.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gtkutfijz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gyyfmgxrl.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/ggbmwbakh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/grhljhrce.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gqprzlyrn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gsxyhnkpa.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gxyqtdmty.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gayefauon.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gvymyfybs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gobhygwpw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gowkgbbua.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gwsmzadww.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gbtvdzefu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/geqkqofer.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/ghinzhjih.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gpwnvsvdx.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/grnrfeutn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwulvfeqv.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/ggvidnnth.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gacqfixtk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gexlhsbxu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gjgpvffix.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gteypwjux.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gttfvrnek.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gupplcpln.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gerbcvsfg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gnqdijklt.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gclyklxjj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gksxaixvk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/ghohecbfm.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gbrsnbybp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gwbpsjkwl.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gnesrpuyx.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gitabaxxg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/ghkuhemjn.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gwzdqfohk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gcgoqvejv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gupkvhuom.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gbsrgzqzu.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gmszofrir.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gpxyzlold.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/goodebcnn.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gdmmnbqqn.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gbmflmzdl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/ghbnpgiep.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/ghgnmoydd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gdekvbvsd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gofvuyhwd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gxgdhkakk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvuxhpako.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gfddrjvef.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grcfjalrg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gwwvkgwwc.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmjcycekb.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gwghfjfvw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gapuajems.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gsvtffvig.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/guxoowafg.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gpruajrrv.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gkcwgolno.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gyzidccme.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gykcraavq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gridcuuco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzbyicwwo.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gsvsbhedt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gtgkruthd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gjjtbmpvt.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gyfwouurm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/goygeuwll.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/galeqcste.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gdtbcldcj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gudblayuz.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gbdumskct.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gngdftqeh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gdjwhowjg.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gnbniehwu.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gbvfgfmon.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gdheohlgx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gibjvslah.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gsltwgtua.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gqwerlaze.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ghhmfjyvu.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/guqrwjhcm.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmylpdqze.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gwsraahad.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/golvapizl.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghvgnksnu.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gnuhgjuri.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gohqokerh.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/ghjistuod.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gvejmaoll.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/guxktttxy.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gnwcbjbkv.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gldtheqaq.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gaguosamp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gqaaqeyxh.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gdrvqseoi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gtdmnmcud.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/geswxuvxo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gombnmhaa.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gcnhcixrd.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gcafsghha.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gnxudsuxb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gnjrndyeg.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gffoklnrr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gqrvcmllk.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/ggcvjllql.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gqzokfjmz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gwifieuyy.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gartpnitl.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gypyhrker.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gkcsqylgu.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmvwlikts.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gwgxwveao.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gfpjqebgx.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/grfwpgxgd.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gnruhttyp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gobnpyvpk.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gztuauueb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/guthymkee.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gdlpnipwf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gzvjihxrx.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gjdtpampw.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/glikxhyph.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gqkhkqoru.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gazvpklic.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gopvciamj.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/grltefuzs.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gwxqvzwat.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gygbeykct.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/givaowjfx.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gumbgckcg.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/ggebimeuw.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gkqbhpwgo.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gwtlslbtm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/ggjlgxxqi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guukmyhlz.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gbtnffwlq.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gepozrghl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/grvgrpgvo.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gnsjvfwqt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gbhtrbioq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gonvrnzej.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gtssfiklq.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gusfybzfj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gykfgdhyg.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gmfkllimc.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gcpfuhfxi.sHtML


<!-- 参考信息 -->