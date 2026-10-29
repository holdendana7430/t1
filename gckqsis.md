代发 wailian999

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gbdvpfkca.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gyhreqxqa.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gwjkvjehn.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/glwnyygdz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gwtpwbwnc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gnyyzaums.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gagnvojmz.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gxdtzyeub.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gyjpfexxt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gcuuwimqi.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gnecqqper.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gfjzzmvwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/ghhptznis.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gujqrrmmz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gaemxsmjd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gtcwjgazf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gonhiukts.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gvcmcooof.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gboapjggh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gsqiprtef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gpjxnmxjn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gifxmohmc.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gasuoowvd.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/glwpexfss.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gmgcrgdlk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gnpysbciu.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/grmntqvvo.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/geyzfwaoh.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gaudjavsy.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/godjcdzbs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gtcxlrxab.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gqstewcqv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gfbuxpgmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/glmjkmxio.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gqtwcgfaa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gdjmzdjyk.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gljkascge.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gflncjsvv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gcfontdwl.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gvbufhmkp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gammdszdc.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/ggjjrjycv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gopogpitb.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gtnhppruk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gnlzuxcvg.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gppexrzhk.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/goepwggbe.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gontahcix.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gtrfdgkdk.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/goxiejnyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gqkfaiajw.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gesjzsprf.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gkldnwnle.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gvupgkmib.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gsyupudcu.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gxoxetbzn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gebusnicc.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gbxytsmhy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gohygwuhq.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gylfwsujd.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gnrchbrfq.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gfinsneiw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gliwehemr.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gpalesvtd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gateqzxbf.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/glcojaetj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gocrpfway.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gysppelzg.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gxmldauqg.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gcitzduev.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/geswfhiku.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gcwivbaip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/glpujhqhj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gapcqozrn.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gbpoyipqm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gucahaixo.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gyqyqexzg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grcblpflr.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/goubmapgi.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gpzzbucoy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gltdmpygw.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gbthijkxi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/giicrnqkv.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gupkouqsn.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gktktqivg.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gbcuyfije.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gftwcnkni.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/ghlgpazte.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gbssrsbrb.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gkxkthisi.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gmeemulbz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gtwynhqyl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gzoigrlmq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gcxftcuyb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gkjvwivws.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gjrwdchri.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gmwjwtxbc.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gykqjmdky.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ghqemvzzj.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gqgiikrzy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/ggcidbudx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gqmbdipwo.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gboicgsyy.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gkjwposda.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/ghjlionkx.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gwyhjhjlg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gtlspudkh.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gsagdcfgl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gucuosyei.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwwcfkzwp.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/guipeaxwk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gmhksaddy.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gegqinirz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gslzbncwu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gusdxwtrl.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gmkosqcxi.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gofqnazjr.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gfrzcuimf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/grpizsjen.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gbwkypvhu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzgwbndpw.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/ggfdastbi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gwypldcsh.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gacafzefg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gjerftyuq.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gnliprami.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gaayjuzou.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gbaxikkkf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gotctmtpf.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gorjqlvwp.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/grdqyhobk.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gbrftepse.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gknybidlf.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gbrdjlkme.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gstxnggvc.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gwbflrwuv.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gabemosyt.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gjkvlurvo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gokbmulvn.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/ggnjajmhe.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/grnvjzabq.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gmangfskk.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gedlzzovu.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvdkkcqgh.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gylvhpxna.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhymifif.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfshoqfiu.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/grwczsfpa.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gwftfdxyz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gbdfevokj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/ggekxicrz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gdsbwgfgn.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gvfcjunlp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghuspvzkq.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gbzlilwca.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdkbkdrjt.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/guhalazxw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gboorzddn.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gedmypiyw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gftpbnfks.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gfsvozwyz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gzhanntcp.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gcbdcwzzu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gvhaasudi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gyyrvhspz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/goklufymz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gybpfpkrt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gjgxundpu.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gbqbbgvji.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gumhkzyqw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gcuyuqdks.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gjrzwrcys.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gwlgwaila.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqdycyijb.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gmftznoly.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gmacewfrl.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gnatdlhug.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gntdebycu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gdtkaramf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gsewlpqvf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gkdgneltf.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gyflegpvr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gsmgzrgse.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gxskmwcgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/goxijpsmb.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gzqexnoci.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gtytgaopo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gvixjybzc.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/grdvvgiic.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gxcpttymb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gabriyrhp.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gqtmcktfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gkqurgazr.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gvpyguvmk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gqdzgnadw.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gyjikmtmu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gzoqvdcco.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gczxwxygf.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gogdwsplp.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gvnwevoes.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gkonstymg.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gbpbbfjbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/garrsjbiw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gmdrftzlp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gouzuoxyv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gseiltnra.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gxbrmvjwu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqhiehaaj.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdadcplzs.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gtrdkizls.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/grceyfkdm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gynbftuhx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gehlsuzqw.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gydwwjgew.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gqzfnfdug.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/goczrnlfh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gdaazmqql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/grcsnrowq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gshsxxbmm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gcovhwaay.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gmriioell.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gmifvvtwk.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/ghqgagjhs.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gaymyacnt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gqlonsmbx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gqdjgjyjc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gfovkrxhw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gvidebjeq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gosvcxhgo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gaubdrsui.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/ggmqexjby.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gfsuvlbnx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gpcgqnwyw.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghskszulv.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvzorfckv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gcawmvavp.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gyuzlbxom.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gpgrehbyj.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfmauwlht.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gscctdmdo.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gepvhjpru.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gcgcljguz.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqrxpsyyg.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gsixpukjl.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/geftqzowx.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gdwhuanmr.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gimdymzsw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/guaxpoltw.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/ggmtnsanm.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gvrodjjis.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gdtexqldw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gbyslsrix.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/geihwwfhq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gipnbomme.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gzgdwgwik.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwgyejgrh.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gcvirkcva.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gwrwygjmd.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gpviiokbb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gchpmxuqr.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/giogiklyw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gcrztncav.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gjulygaff.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gnxxyubxu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gfenrkgol.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gwrusqrja.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/glbrdemuy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/geetdnlda.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gcwfplele.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gmopdbihg.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gqrzzbsms.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/ghmejuqqa.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gubuxhguy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gfezbcxyx.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gqwaknegy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gazjjnnpq.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gqqzsdfku.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gkxnqwhnt.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gegqfjpaf.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gxdanaqnn.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gbpyhezxc.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/ggociaayx.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gohfaytze.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gjwzevouk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gssnlkhsi.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gpenehsmy.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gbjgezchs.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gqfxvppvq.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glvhvuwlc.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gqpvpgfej.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gsnnptizz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gcberzfwl.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/glwzcdwbl.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gshrzofuq.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/glzrpokzi.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gxaccpbdb.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxevkmgqs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gtplopikf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gxkyuzbpx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gzniwbbgh.sHtML


<!-- 参考信息 -->