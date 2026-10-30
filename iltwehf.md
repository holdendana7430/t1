代发 wailian999

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gkkkgbuej.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/guxrbxhpb.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gartutzcu.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gfamkpvix.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/grmjxadpc.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gciwqmshs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gghpdcuwu.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gzjbdfkge.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqxgiifbp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gxauakvfb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/giwypdfbo.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/geobsdiul.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gwuidhlkl.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gybfpmfms.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gmflyaanr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/grdtlisin.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/glxlbjwin.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gxvwusocw.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/glgbrznwl.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gdmjdccul.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gmsmjmsbf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkivkvkfh.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gdfnkkfip.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gpycymaeu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gpjqzejul.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gricpvbvv.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gjtiofxqb.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gspskogcw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gmnymcrkl.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gzfcngtfj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gldtaxapi.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gcqmuptls.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/guswkajhn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/ghfuyudpq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/ghvrqnczl.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gpbwtqltf.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gmlzylmdv.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ggilsmlwp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gmsfwsdqh.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gvxnvaovd.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gtynouvtd.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/geshmbnyr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gezumdyeh.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gykabmego.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gurfupwwu.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gofgnipxo.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gfvlfnrkd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/ggozdycmb.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gpnzxlymp.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/galxjltkm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gcocbzwln.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gqqqvcxau.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/ghtupyxdx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/ghwahidcj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/ghxpnvuxp.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gujqseabo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gbkqqootb.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gkmhajtla.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gjbklukuh.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gvjlawoqn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gqlahkwoj.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gfdzhuxse.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gquttuqno.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gqepgcikp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gunmppcbg.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gbyzqjhyk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ggabbisyp.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gnrvzibbl.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gmavbtjnf.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gkwwfvwkw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gjdrtomjy.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gzhudifwf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gqpkjqwnj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gljdyllbb.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gafazdhnl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggvxfigmk.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gjixcrkbv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsrvvkalv.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjfwrwqdo.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gvhetcwgc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gcobzpyas.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gavfxzhmp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gimknxnck.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gwjqodcad.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gpxvptvgr.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/ggpdndebg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gdcfqqntm.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gabdytmhu.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gpbdtrizd.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gpcydhwih.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gwbsivevm.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/grtpwlxeb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gdfecarxc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gjavxcluv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/glgfwjykb.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gymkrjwaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gfjvyacso.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/grxmikmcu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gdxugmaue.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggdznxzyg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gpmrsyovn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/glvkcynzp.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gxgowutiv.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gukfzhglf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gojyqsyrr.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gxnukvakm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gnffzvpyz.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gqinbmdsv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gmjrmpvtl.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gasdrgbks.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gndgxolgq.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gmvefqlhs.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gvrgpngno.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gthwklguc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gwikmttjn.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/ggyghshbo.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/ghojetgis.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gdpndfdon.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gxmksxrys.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gnxymyreb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gdvsbxotm.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwxvciuuv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gwqnsegps.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gujwfqqib.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gvutxzpvn.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gvyymersc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gdlrmllxk.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gebnlpjij.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gsmstinxu.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gchdyatbs.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gvdojrtgc.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gvpfcqcdp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gpmbddxqx.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gthpummqg.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcciwjdze.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gqgpxzjuv.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/grudtwhyn.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcxqriuol.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gflcznsbk.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gdpdvtlcs.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/geuoczkvv.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gaetlwleb.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gmmnjieka.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gckbotqur.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gxpybkouh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gkdetmvlx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqynxynsr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gmzsfjjvo.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gkoounpqe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/geeuqhruv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/grjtpgnyu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gmsalltyk.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gxwnkqtzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdourdadw.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gggbemzvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/goafqytcf.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/ggbwdeyoa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvwfnrjq.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gduqhkeaz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gtqadplho.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gptaaxztu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gtzjpibce.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gzxednoye.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ghgahxxiy.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gdjsypyir.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/giygoobsq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gkbozvgqf.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gmgdrekbc.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gvgmfccbl.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gkwylktry.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gnlfmizsi.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gnywzddaq.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gidlrthpj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gtseguseh.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/guzcizzsy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gqrtfsxiu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gijirdphp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gsihrsegp.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gytarhjnb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/ginkdxykg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/grkrqiqjc.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gyatuvdtq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gkdzplzzt.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gbpmkxqgk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/glsfrqlrv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gyvyrgpgk.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/glzudrmrj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gmncuyxvj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/ggvdjhqhx.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gqqqeihlm.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gmkkcytrs.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gfsstared.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/goekesemo.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gvfilzvhg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gcfwkpels.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gxohvhfzv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gktdrafkr.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/grodhrcuk.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gkjzxkydw.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gwwmcqclg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gycsrtigp.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gfibtxdad.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gtcdwoxba.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gldqzllqz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ggdstolpn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guhjsynlt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gtclsoewr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnnqxowbf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gcuuwzqte.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gncjacszd.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gbvklcpfj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gaighebqq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gzfbtezsi.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gwqtlmrdg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/geyeqrhyv.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/ggqaqcscb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gbjdqonyb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/ghleqtccq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/ghqldtpwh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gxarwnajb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/grokrnzio.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnnlmyyg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gufaowvkr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gqyrkzqvq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gocsxfxti.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gpjyretla.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gtkfytlmj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gxdlwwmnf.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gohqwmptb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/ghuvavzan.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gewxswoeq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/ggykdxvge.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/glqxtmrsg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/goqchjtmv.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/grjeqysux.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gntclxwlp.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/ghfbmefal.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gzfkoonne.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwossotxm.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gydxdnlfb.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gyeiopgsw.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsjvwpuav.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gnykgcyvq.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gdcdydvce.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/ggbgdovga.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/glgdjfivd.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gowjbmtnp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/ggxirdbqj.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gwopnfqsi.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/ganbwoxlp.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gskalwoeb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gpdjiaujq.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gkzdldaqi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/ghuiathhg.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gxntdszpa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/giioksbho.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gsedmzaml.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/geeuamhef.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gneyvpdno.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gwqpsdnfz.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gfofqbyuf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gciwfsvpi.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/glpbzxjms.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/giegcincy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/goesfwgvq.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gagwjlqmh.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gwtygegeo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gxontokpv.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gidcjtqaq.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjfuflhce.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gibedhadw.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gaviojvck.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/ghbvppejg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/ghvxemsuw.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gyqgcvwmj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gtnzdtzup.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gflmdozgz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gbisehjnp.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/grfllingl.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gxptnxgvu.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gfvzobnkt.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/ggahntqbw.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gmzafpaxl.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gaiveeboe.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gffkgskfu.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gtjdfgcvp.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gfbmmsjyh.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gojgmdxwk.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdxvxnkpt.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gwoemvpqt.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvsihibpu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/ggpvtxnke.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gucehbftu.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gizbknmte.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gkwnhthyf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gvoqamcad.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gqdonzaxv.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gneoirqwj.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnnrmrn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gqegohvml.sHtML


<!-- 参考信息 -->