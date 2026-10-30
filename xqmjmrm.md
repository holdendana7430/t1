代发 wailian999

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gccaaiwvm.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gveshfuvq.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gyipjpeje.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gdxfadaan.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ghwzrijfi.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gnjnmsyiw.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/glvhaujqv.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/glemeaehf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gihwzmjzd.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gxmluqtzv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gshweewie.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gguafcgca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/ggnldkdfl.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/ghoypfnfi.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gawqnmpvp.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/geqqskoys.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/grprwlyae.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gzrmfqsfs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gzgdctosj.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gdgztuazf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gkdektipv.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gdqpwkvyj.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gnrepvewy.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gvnaccusl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gwbulrdqv.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gmvbxzyrj.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gkvizpboc.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gluwgqidr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gerkxjtmi.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gmzdgkszc.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gbephpdox.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/givwwjsok.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gnxjoxief.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/groclmevp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gmvavlyuu.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gqmtebnfi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gpjhtndfs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gfwbospxk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/glxtgztgk.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gmtqkfcle.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gtqtjkuhp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gispgpyxf.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gzthdblve.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gkxscrpff.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gxikrjwxl.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ginrpkqoz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/guxvqjukt.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gouwgvxrq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gzgjkvryi.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/glghsjdzt.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/ghyolokti.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/grvizcykh.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gyzfweitm.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gcbpnbohz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gxxpxbzjz.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gyqogawgi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gxhgvawhb.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gqzhotzmp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gtxuriaiq.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gilfxtdwz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gwbqzflqk.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gcgsjvobf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gkfvjuwim.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/guiqwbdqa.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gjnghyavi.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gmufeovnp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/giculaxeo.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gebrswcgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gprktisou.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gphmwbwnj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gelgsmipj.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gjqiuxseo.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gjiwqfspv.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gwyponxcd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gmausiggh.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gimiybqaf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/grrvqtopl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gaycmmkhw.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gfikkqqls.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfvdlfapd.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gnfntrhvz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkhtfjobm.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsxdbzuyn.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gprlngjnd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gqjmvacfn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gnoubimxr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gqjkivnjb.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/geaqowcir.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/geppgyrqo.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gujszodih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gjpohfbnb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/godpjrtfu.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gnkmsusst.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gbqdkwhwg.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gwuvmwwih.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gflibgmzv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gpiszbkpv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gesxmxmrz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gnpsnlbai.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gisfrzogz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gzqbidolx.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gmkcfubpv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gaqpanhpi.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gkvafsqza.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gughwuvwf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gdmlifret.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/ggtzwxzlh.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gzqdhketn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gvrbpkpxd.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gxyetmxwq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gndagjgpu.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gdxpmvoxg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gngihvjvp.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gpsagrwrc.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/ghrkibymy.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/ghabprizz.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gdviibwmw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gwlbndgxq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/ggzlabafh.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gqtiavzkb.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/grdslywrv.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gqukzsvpi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gfzcedhly.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gnnxdeidn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtmjwlmmf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gnwkngaxa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gububmngk.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/glnudeckk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gomogmgij.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/geaihcdgq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gawzainbp.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gzcykwoxo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/ghtpqkqtj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/geqzvpvcd.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gaqyfizdy.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gdfwrpmco.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gzacssvxb.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gbweogfoz.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfzdwlepk.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gvxomsjqa.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gvfpochiv.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtdhpnw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gxqsiweoi.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gjgrdynsv.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gfzzlrsji.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gdhfykqei.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gpknprdlp.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsvgkrdkb.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/grlszmimu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gjambwcwh.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/grjxxklfy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqkowdfod.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gmlanbmug.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/ghceaqddi.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gsqfbgfkf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/glazwbjvu.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gwaezxirc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/goscpxddd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/glgyaqrii.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gomaijcvi.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gobluxqne.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gohnzbdcz.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gtsnbfpfv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gdymansnu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gpdaqxlbs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gnaqherpm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gzyolviht.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/glbgpqscs.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gjurawram.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/guxkbieup.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gllntuqjy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gymiopwka.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gpcupkpci.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gcrhopkmk.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gpxshlhhv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gxiglfzzl.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gndxndwkc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gigvwkwyh.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gkqeakuip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gzvgjdhmh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gibuhkxsu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gfmklyqat.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gfggtunij.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gexgwjhey.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gmgjvykmj.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/glmgranie.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gcpqqquot.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gttouzozx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkfxufbhs.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gxbvawtpb.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gddiicwyo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gmeyghooj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/grgvvsfni.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/genwpbrkh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gpsbmmwvy.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gpugldrnb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gguukhpnq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/ghamoszck.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gtohlxpwa.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gckecemwa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gkdcounut.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gmplalzts.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gzmkomjti.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gkehsmxcs.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gyrufovgi.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gvnpejdbd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/genkudajo.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gcgeemzix.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gcnjyyncj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwldajhhq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gvwrncqrs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnlxcufro.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjvwqradk.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gyduwxxdv.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/ggobxpuqq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gwfqonrnu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gegjpxcap.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gjbmybvta.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gxbqodbtg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/grjmslrok.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gcyvlfxhe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/ghlvlnfir.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gngxwzjfk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkgrrgzmx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gvjbxkdsp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gzhysmvef.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gavqdprqy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gplmlmkws.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gifseqzzd.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/giordithr.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gzuqyygaw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gitgmmgte.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gpjztwhsf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gmkerpmpy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gkurqzgvo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/guzyfvqqs.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gizexxbad.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gdviykjrg.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gmtdzlnzc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gdlwieikx.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gpbnntbbr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gkajuppwg.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjvtjdhay.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gckpvzyll.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gagfwnsyq.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gdhrkvbjj.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gvfflsoqy.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/galdeefab.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gysatwupg.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gdpxxojpn.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gghymhwxz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/ggnqcncov.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gjtoxfyle.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gahrawbmg.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gqcrseeuo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gfhrqdklt.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gviqdhpdy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gvamyrwlz.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gtvogyflp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gxxvuffux.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gwfjwntpb.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gwzgtsrbs.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/ghotpzddj.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gaunsouem.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/guhpasywk.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gzcuoekoh.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gbsxwbdsp.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gsylnopyv.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gelbxhevt.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gfrsjfepl.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gssgiydbw.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/grvaxiswz.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqgkxkeoo.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gwanfxqar.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gnupftxil.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gyxzuaiov.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvtrqvjlg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gdbscwehr.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gqurqxgvj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/geaayhbhm.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gwdvcbczr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gnnycxsfi.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gghfdvkvd.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/giwxorkzy.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gutyfmfjp.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gbwijcaro.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/grspsucar.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gcmdzpuvl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkiyvnqcy.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gawbucrwd.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/giocqrhji.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gpjgwbbmj.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gocmlrvsa.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gharorglj.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gvsiplfwn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gsxvkzkyh.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfctnolmc.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/glpuatuft.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gbcwfvpld.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gnmbpnxyw.sHtML


<!-- 参考信息 -->