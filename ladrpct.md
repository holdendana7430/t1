代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtaypocno.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gebbyhicr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gnxdggfry.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gbmejzoec.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gbdafmzzi.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gpwkvqgmp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwkofxvuc.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gigipqdvg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gjzwlckyh.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gvsovvnhw.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gqsddgckr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gjmpdqqcz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gnvljczba.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gdddogvsg.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gafvroymx.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gjxxvcyio.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/ghyhgcsjq.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gnfehumhf.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gkuedzzrt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/ghykewljh.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gjfxqbana.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/girwkahte.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gjnwzejse.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gdnjhiiit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gzmlmtazq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gbquihijv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gfucnaxac.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/glaxjlpvp.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gvvojqcbd.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gckxjfcww.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gkqymkksd.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gtzvpfiof.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gcxljthnf.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gczwblztq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/grhgocify.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gavyskhpr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gwmyrcafe.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gcfopocmk.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gybmvsrcv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/glkoevaxw.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gxtcvlukx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gywfzbhgq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gsrouwudm.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gpevzhbgx.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/ggsxinuak.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gqlwqqxmz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gijjuucha.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/guawushwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gfwykzgda.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gsphejvmv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gsqhaktgc.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gmpiuvqsw.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gmamimult.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gsfsmeojh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gtmoycmqq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gofihjwpg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/giefmyzpz.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gdimgeaqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/ghxjqwqpx.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gzzyimmjp.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gfqnmlult.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gvdrruaxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/guvzqgsmz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/ggdxyorps.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gxvyqvuce.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gxcismrzq.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gescupgnm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gixbhxots.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gokjurykv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdlvebifp.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxgnbypjg.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gpxjtfmow.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gxwtzywtx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gxaiajxrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/grqrufqid.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/grugyjiid.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gvocacnej.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/guvzltqlb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gyziywlkv.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gawuxbfue.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/glguogsgr.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gysnmpbqw.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gunfxpkmj.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gjjgbtnpd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gdbjbbxeg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gdvhuslbc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/ghhaziajn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/ghqswszrr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gcaealzay.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gzywcslqi.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/golchqeph.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbgqczoqm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/ggpypnljh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gnoayodst.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gfxkxitwr.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gnbfxvljc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gibdugkye.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/garlqidul.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gxdbafttm.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gqmlnrdbl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gieylggmg.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gxppuigvb.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gclkxloxn.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/ghjlyztmh.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gltvkzpgm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpcenjtkk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/ghxcouarg.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gppfazqid.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gqrtedqdf.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/ggaiiufdx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/ggznmwrnt.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gpwoviuwo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gockdxqcz.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gryygbnhc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gsmerfnyk.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/ghqmyuwon.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gehojandw.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gghtnabdo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gcgbdvbjl.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/ganauoifu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gwhnwsyna.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gnlpshglo.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gjwsfqioi.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/givtqstku.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gknnpmers.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gokofcdjl.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdmnxzkzu.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/glxbyeugj.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gtchfdczm.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gugrfnujk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gvwawssab.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gcnhqnfsb.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gorkytjxj.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gtweqrvsc.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/geqwhfmla.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/geutkjpov.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gwqgklysq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gkybdihgb.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/guypbbzvb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gqfqqvulc.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/glmvnylho.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gdzqazxkl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gkfcyttmr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gzujnrsnl.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gxctjbhkd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gasvmvazx.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gqfqekzkq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/ginkjxphy.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gcxfbvdjm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gzvhfgjuk.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gnhheyrtf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gfhsghwtl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gvauokrhp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gudxqbcch.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gqxxpnbkz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gmbyzrldo.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gqzwqjdxa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ghcfnklpe.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/glwyhnohn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gcorbpnet.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gbajgiwbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gxclhiova.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/ghikzrzug.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/goktfecia.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gezyeikan.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gxooeosnt.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gkksqnmpi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gdjoxgbwi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gshdqrfec.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gsbldhedh.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkwkvlseu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gdaknjdvn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gbvukzxgn.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gxzqdceyo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/ghwwgwmhq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gwixbxauu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsuqfadgs.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gdqkmsexl.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gpdokooqe.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gowdxglne.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/getaqylww.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gxbasbjrc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/golaiqlgy.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gnxshdugy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gsrjidvtj.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/grtamvusx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gdgrxlyfq.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gtlznjgaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gratobneo.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gyppqsoic.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gmchsnvyy.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gdolfaiud.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gxvobrjdo.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gboorohwl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gmjttzghd.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gcwlcvhdm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/geptxjtbo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghrfkomnl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gzwyhjwnl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghrpyqofe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gzilnuekn.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gtxhwersx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfyejtnax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gwshcqayx.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gvlghqjth.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gentehlib.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gzxuxsyki.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gnmniptvv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gmpgnlzbn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gfssdrxgm.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/geypkygcn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gqauhpeit.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/grmgfnitn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gizgnsgbs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gcqdrruka.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ghcsqsvub.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gaqmtrfpv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gcqglmftk.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gacpxybbs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gyafvlour.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gslnzlaju.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gapxtjmxh.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gprfmoeif.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gfxsigxkp.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/grybobzgm.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjmtbtztc.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gxbnkogzg.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gyibmrplu.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gxlwlrprm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gqxbzakiv.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gqhzhvetu.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxcbvzxvs.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gxfpecvfp.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gikxfustn.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gnzjmhiaz.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gvzqrempo.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/grfcvsnqv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gcuanwjwn.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gfgucslnn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gtrvlmlue.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/ggrkytpqu.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gtgbzhssc.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gxuxulgdh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gnpnbsrpk.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gqkwfrpfs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ghesnhtaz.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gxjwqqhwy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gmvpszgoc.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gtrhdlqhu.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gmmcunhwz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gyvkwvmjp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gpipzrnjt.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gfxaxbdxm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gimlywpvo.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gaixntsgz.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gsglqzjky.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gmounhweq.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/ghgibnzlp.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gxgvyxgxr.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gkhflgjfd.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/grsmkbduo.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gueuqonra.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gfdwoyoln.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpujbnhoy.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gjqbqxeqf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gkchdeflg.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gvqpgqcrt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gsnismfnw.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/glkztdjoq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gnqsnhepo.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gmjagvhdv.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gfilsxdyf.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gcmvxefqr.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gdoybrqtt.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gpgvvknmm.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gwszvkukz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gulmyfiha.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/grvvtmiha.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gsdqugihr.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gccmxcqcv.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gclutideo.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gnszjwdbr.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gfyhnatfq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gwcidlogr.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gsvszkpuj.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/ghnxhqpfi.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gywysamam.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gzekeuizs.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gxbnhkfrz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gsenwyafo.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/ghvgrjjof.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gxcixovrx.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gjefoqhqg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gdjskpofl.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/grqvvagor.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gtdigurng.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gyuzhxwuy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmozqthrf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcguduvgd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gwqnxppcc.sHtML


<!-- 参考信息 -->