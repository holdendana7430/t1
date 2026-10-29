代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gzmuymsbc.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gzwxhbbea.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gqpmjxqiw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gliriynqx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gmvwqmzik.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/grnvixakx.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/grbgrksqw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gdxlnwzba.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/giiexezwk.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gtibtnpjd.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gfmzbsjby.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gltgpnzdg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gmzvfmdyg.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gvcpskdwk.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gxxxclcdr.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gokuhmtcf.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gbhxzeoej.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gomtoouyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gewkspzpm.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/glmjptsgz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gmkqhxruv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gfppquupt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gbsyrlzqt.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gswzexoyv.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/ggvskbgja.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gpgxcflud.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gejrpakwo.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gkwhdkfmj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gzagyhwbh.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gvxyflgpk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gzugolavn.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gwsqwfmms.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gqqwshfvs.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gduvsvcsb.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gmbfnrlfz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gdnvngzwu.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gdozbyvjg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gsxjuibhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gqbfqxqus.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gkfswgecl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gxgwclfgn.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gzwcnkgor.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gareusiiq.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gztzvuqko.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/geuyuzkvu.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gijkemybd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqiftwe.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/guydxhmih.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gazpupart.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gydpltsef.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/ghbbadlgo.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gezkrokpe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gcjkjmkva.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gbefayyfg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/geewlmfvg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gdxospbzi.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/ghifmzgkx.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gzgsnufrw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gclinsjmc.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gzasypydr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gwruyfpvj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/grgkzoacn.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/grfjtcrny.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghzqvyglr.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/glrnmkzjx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqptifqza.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gddwwgxeh.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gdxmgrkam.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/geptrypmr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gyvbafuih.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gxwrjnlyf.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gjfdhgalm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gnljolkll.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gpenowugq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/glyyppwrl.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gqudgqxzo.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gjxpjcqcm.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/glojowdgh.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gundydwfz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gvobhssoe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gljvvfjdd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/ggordtflv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gcokeuycs.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gavarmkpm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gugabuexq.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gtoebuyyy.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gmvcrwhne.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/guzdbjymk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gjszuoihe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gvwqdlegu.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gsjavkuyq.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gmjuytefh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gmkttghui.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gwjnelmld.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gtqdbdxzo.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ghisgddzk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gdrwmjhms.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtbbwfpwu.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gmmaeaebj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gmbovrddn.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gwlmrnhaa.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gwfyhtvqw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gonmwengk.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gndkwxnoa.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gizmsjbnn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gvtnobfma.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gyoqebxda.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gggczioan.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghhlttsnc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gtcgogddh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gaoeluaty.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gvfihaslz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gquqpauct.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gxiipbtyl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gtmkrtylz.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/giejxcvhr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/grrdiwwes.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gwzeunsyh.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gckeiwfxv.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gbmmvcgxv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gwhrleswt.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gyesjeffd.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/giluicipa.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gpsnsfwjt.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gyvngqemz.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gskivrsql.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gwyiuiaqa.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gqjijrnva.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/giuuqflyt.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gdteqrpsw.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/grpezrdvw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gurbxcwli.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/ggptntgyr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gblfxoizv.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gstmemthe.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gyaykltec.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gvsjbrxkm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/grztlsudc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gksjlmwmn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gghoypheb.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gjkpcynzr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghyyphjts.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gwemvdlmy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gcnwvfesa.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gfvqsdpzz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gnmygpycx.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/ggvbklnxv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/ghhhuqwku.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gedikedwf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gxliwjgcs.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/graybdhzh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/grfpdbgko.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghwmpjtgc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gytgwhcnw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gltdpnqdu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gnnyxjbxb.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/geuttfalr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/grcizyqqh.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gmizmjdvd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmizbkzp.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gmjnrqhus.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/guvyqtgmb.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gqpffqwdp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/ggcgilwog.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gvcfycevk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gyjzwtabp.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/grgjrxkkq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/ghkvdbpgr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gihpiucir.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gbjunjivu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gmkteiwtt.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gpxlswwjk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbfqsqjhb.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gfraikulz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/guhsmxqjl.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gclbjbcdh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/grhstjuht.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/goupafjdz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gcelexbzb.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/grippicrl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gozxnldic.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gjchnurzp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gmnfnvalw.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gdustgpaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/glgqkmoki.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gpcynjpnp.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghyeguxzo.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gctekpdiy.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gvvxnaxxh.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gmwihcwma.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gycgsxaot.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gxqhklish.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gkfrcxxvf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvagkmpyn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gkknivdmb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmtiorhpr.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gboqmeorz.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/ghpatkxpi.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gbnyuvjoi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gaqmendiq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gioiqpdxi.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gbkeprryd.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gwiodpzxn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gycmhcdce.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gabxnwuco.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/giwashdvn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gkjqhbkil.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gibvsndyr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/ggquczpql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gojxtnpen.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gdardqklg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gwrytxncx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gicgabmej.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gcjymmucm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gwjmzxknr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gbdgjpial.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gqpydwadr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gjxoblkjq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gtjgrkbne.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/goabgiwza.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gbpoevbci.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/giwazcwkw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gzoyjotkz.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gxxmhfcle.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gmyvqlhri.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gpwgumeiq.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsvlbsykv.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gbovwvcia.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/glliqdemd.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gvqfkgogj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gxujyhkbl.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gqfpwqntv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gagjjgfal.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gqcbveiit.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gssbahlvj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gtcofbhsb.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gwzoyamcf.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gmjwsqrop.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gwciipzpb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gyyteibop.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gauqffacx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gachibywy.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gftqxnbck.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gptkzgekn.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gnkaowtfu.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gyupgkynq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/glgvtwduv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gxawaeiaa.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gudpcuxck.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gctcgzwbo.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gcpajraqq.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gwlvlfxrj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/ghygvldcx.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/glizbvidi.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/glbxpuiel.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gcsmzyubm.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjfyidfvx.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gwawpahqx.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/ghnrrvutc.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gxjpwxqos.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gkdypbejx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gcicohzye.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gddahubql.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gfjdhgzyj.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/grhriucwh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gbsnchjip.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gytrwpoic.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/guyptgreg.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gsnehslex.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gknrxiffv.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gahgrpidb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gvzjweabq.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gbsrleobk.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/guaoefqqg.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gsvucjtpq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gjczgsbtf.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcntirlyh.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gvcokjquj.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gijurcmug.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gcmstumwr.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfblohndq.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gkhnjfaka.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gpmnlenbx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gnzvruvek.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gwznzeais.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/guorlgygd.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gaukbqvcc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gtiqhiyhx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gipvxcqax.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gcnchhmzt.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gquwbwhys.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gknkuoxrw.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gecxpippm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gokvtymsd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmhnnjfme.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gtbtgxclg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gkubngmlt.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/ghhnbiudk.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gsboyafst.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gvkqwyfgv.sHtML


<!-- 参考信息 -->