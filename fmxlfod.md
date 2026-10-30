代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcjkcydy.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gpulbwfox.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwiuvguo.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbwfysjsc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gusjklxpy.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcysbpvo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtnojavgf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlqhwzkm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/ggscxpipg.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxcnumci.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gycjgnadn.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrpdxzwg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiubrhna.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqtfxvu.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsttjgnke.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ghelbdiif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gqukslrsw.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvllrcar.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvrmbiio.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/guujkawax.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gywsuyowp.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvpdhscj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gnkrrtfkh.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxfcpoix.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnynsazdf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gltmozjqn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqymdfxg.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzmrqabmf.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkttwaco.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqlhlpryk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/griacdorr.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/galzeemdk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/grpwftydx.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblvozkmc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzasoveb.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwhnejkj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gcxbmaaal.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gbeiblvzd.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjnnvris.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwtsyfh.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gabdxvezi.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganyzksay.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfiuzydv.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfzrgsme.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzopdmkh.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gxezsyxmg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzctntal.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/grvxfxwke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gclboxcyo.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqapvvjh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxdbumluk.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtpuddzt.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gsmyxmoxv.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/grdamyryq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggumnhnhl.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdvpmldz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gdkthpqru.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grshwqgpt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukbblsn.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoutujpq.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gzpmlmhvh.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gbnrpomls.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqfnzgga.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gwfldhoqs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/givqiconl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/glgkgevdl.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/grmifnbzl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeflhsvi.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/geialqynv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsjcqmep.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geklqenrg.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztkclha.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gncnifhgr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpifctedo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gbtlnvpes.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaejtcdj.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/grhxganjo.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/golnbcwqm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gumnicpnv.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbnntazc.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfpmudn.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gbtzpwwkr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzddfbcax.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyudqcxop.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galsdoblm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/guypgwqtk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/grfoabrnj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhclnman.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gjzeyzldd.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gneokanab.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmokllwr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxzvpbdn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvjuexc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykiuuvlv.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/goimwyney.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyxutubd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfxrwhbg.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfzmmwip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubthyknn.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gdjlcawxc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gytrernxe.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfsgkyhp.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gcdshkwgq.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gshguoeno.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfibwfhx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsdpmrye.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glocwmfcf.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbiwzuxyq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/glmkrhhoq.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyxedgxe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glpsfepun.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gehvhemaw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gavjemqox.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/giwwhyobn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqarjkkhp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvharltv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gwywyuzcn.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gpvydgiqb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcecvignl.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/ghuzskfxr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpmtcahm.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gsbqwmzhk.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gztfhnrpd.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgakbjxy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkbzyxdgo.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gibtsfxtl.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gmpnoiolm.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzjgkmrj.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvhhkeht.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzqczxagw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqytlers.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/guyyflwuz.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgssyedo.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfgdypxo.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gerggcyos.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmosvsmq.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayzvhkzz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkzsvsxji.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/geejbseah.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/glihfhtaz.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gmiawsgvp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghbwbisbq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjepmfjv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdmogsmz.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gwcybmyej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggubtzcyw.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxliplrqa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfqmlylq.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gepqtzwrs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/giosmlmuw.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlsayyfi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxckgonxy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/goomdldtm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gsxsuyjcj.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrvfgbza.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giipptpoi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gddsobuxj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjgnjhzb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnryfvxfx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqljoxyvr.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gsabripji.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gonjacvvf.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/goehhhhrx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grszlzvbq.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gqazjzjmj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/goofgzpjd.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/giowjhzjf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvhegifqo.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvjthmnz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcphfgndz.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggnxaaibx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gclkslfnr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnayspxde.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaatuevz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gnrcbqwkf.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gridstyct.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswapigkd.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbpxuynxb.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gldhczdxr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/grapeyeyn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmvsauzq.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/ghllqwgnk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzxeirr.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/grftrsuyx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsptlwiyt.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqfaiwhjp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ghoyuavye.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwdamnrip.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsbwrlcw.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/glksihjxv.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqsfvcsk.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvvtxogt.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/grgjksaae.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcgbfuvl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldqsrvp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/glemuzudp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gnhzzdfuw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gisygpdxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gtqwxwdgk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsauaell.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnzdkhuln.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvunxdwu.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galirjgny.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gisfczyxq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuamvcqo.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlwbufia.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gabievyke.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxfaoeps.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gnucbthjm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gexqixfqf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyeeltyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrmxyzkz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gwvvlkoft.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqyzvftk.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/guksjowaa.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gscfulqub.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxnbjdjpc.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gxnlrcjjz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggzibftds.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsusygijp.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gylmhnlvr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnldpinew.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gubmzvool.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gienbulne.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gociixrca.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfnsdjsv.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/giwauxmkg.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gzvoecibo.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gwcettqzs.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxasauou.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwslhzthx.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gcvgtkoiu.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/giqroypna.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnidptbxc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgzujbln.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbufbdbp.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gtajzbscg.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvncfqazw.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/guisbxqgo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/grigmcxhv.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gqcldxsqh.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/grholstve.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gavkgktzj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gycidzbid.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqggmnflc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmufixudd.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/galinktsf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzapguqc.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbaclevq.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbylvgmba.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gsoguehpx.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gliirwpee.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gkukjfurc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkhoyrbr.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gluadhlku.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakmzqree.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywdxclcj.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwgxnbxz.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqgoowzg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuvrdegn.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gspcrrhia.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuilhfsn.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghyemwxqe.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gvakoycgw.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gvhfooqnt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/govmhtlqf.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gcamxkzvw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjokehtn.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gqztuyflq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuqeeept.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqutmqcqr.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gfmpnreqf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnhneaoq.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcqpdey.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnirxqnv.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzaedbyv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/giprruixc.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gallhkhvp.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjuevydi.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxclbqjy.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhfoepqq.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggovlclpw.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/ganqrceqj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcgmegnf.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkrlipku.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsxuadoq.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghetmeyqk.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gayekceso.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/goavpbqwc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcngntfza.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgiunoad.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxqbnroa.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gneibafwj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gidpliwqp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstbqgatg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoqhuttg.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvyeiyt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghpgrggor.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnrotkemh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guouibmil.sHtML


<!-- 参考信息 -->