代发 wailian999

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzdvuofh.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/glvajbfsj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlaaalwq.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guxihxmrs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grlzniduy.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gjkjcywmj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzmmorvfl.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeornzls.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrqtgviv.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzmgsgkc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsguikyxv.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gicrmegwr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gokxgvhle.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gzougmicq.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geezzlguk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjutaren.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyjgxzfq.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyizifoqf.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gerpylhii.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/glnilogpk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkdvdceg.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbioeotze.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gepplicxb.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/ginpqtdmw.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/glszjcccr.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuyabpgc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/goghlripl.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grmeagvss.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gyppyzysa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyvklajb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/garhwmkbo.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gzhxccbma.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/guifzzcvp.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxquzakvj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/grfqrjvsf.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkeokwep.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gzdyxyhwf.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslkkdbxl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzokngwz.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gnpsebrkw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gyipaonna.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdagkqac.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gfgnmipln.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyanzvldz.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqezpkkeq.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gcagitsnj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqcuqzyo.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gchcfynzu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gpjnmiqmi.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbrxhlyt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkikgfgo.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gzbpjqmkq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbckfbot.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gipkzrfgn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfouelngi.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/glikxojiv.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxlaqmbh.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ggcnsblmp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gexeahtof.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfmhlmvyy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrxlyfxr.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpxvrntcy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzlwtaqk.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gimsjexwn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbbkagct.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/ghngpgngp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlnjowej.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gpphxgpnf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geattmtcm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gfajrjqki.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgzwxpyr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gptjuvmad.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gteojvlle.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcivtnejm.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/geabdpthd.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgjqtalv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getpuuijt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkyzmvm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxtvagsm.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxzkiyug.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gernezeby.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ggupzduqm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwifwruoo.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwsfeqjdr.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgkqkhat.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxwmiztp.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gimajemom.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfuoebygy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmiknaqe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckbpwiis.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxwkusjs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclfybjvb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gseapejhz.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbytpynat.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gpuryaeke.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/guiyhtrfc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gircidwjb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gnunzhyat.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzesrqbl.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtntofdgx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygsfvayv.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gscywzsem.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjhfwett.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/giqgbjsso.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gurlbrniq.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gauolleag.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/guytwzvff.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiaafdlw.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuznkght.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdopphcq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvztjjgr.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gurkkxcch.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulpntrx.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwepgpwe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/glmdbhwjz.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gppbbldos.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gscycgwyi.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnxyfloi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqvbsluf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxicydjkt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjmsaqfa.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkhyiyfw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gbhatcdms.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gjhguzrbt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqxtvkhf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxriaqemb.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkazctvou.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/ghwbjpqel.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzrwjltp.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwnotkvwo.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiyghrop.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjazwatci.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcreanzr.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhhhzghs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpseunugg.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gfnnnssuo.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gdhpyhijg.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmchlfux.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gkohntqqh.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpaytetjk.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gzfrvyyfk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhwiqzaa.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmbgdavx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhsewswt.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxnflaph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdybfflz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkypomae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gljhtksbm.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gxgqoornx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gflxmjpvf.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gngphpkvi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagpjvxik.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmkotfdb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyxeuduz.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsgoadbcz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gwuuflrhm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaznvpuv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/goskgtwtw.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvtivcpj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gojaxzzyl.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkehthikc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/glvzxgyyr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsujlxfmf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gnbwrhbdw.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gmskvjsgp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gupssuyop.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gqewgpzri.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gumhjsbha.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmazsqatc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkkykvdp.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gslkihejy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqxpblgb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzzhtdwf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtexayeeq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfqrorjk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtdceimd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gymdzgmyw.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpmjjxnwr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goygvsria.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyoblcjz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmhugqlfd.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwokpllsn.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gapqwbtac.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqsokpyx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpghqgljl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwscrbqcm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwlycbc.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gwhnquknw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmefgbmfg.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gnvjtotvz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/goyihlszg.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqkrjcgu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohmqxqyy.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnqgiaro.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gjhxdblit.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdqkihzr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyrlcxcm.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/grssmikmf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdlskjrm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/giirigrmc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvlimmld.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtgevpet.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmafhesps.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcihqplfi.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfckvykhj.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grjebvlqu.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqchjfawb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheegbhck.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbwoickw.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjwmmbir.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbkyibbg.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gnacikpkx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqmjwoxie.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqbothhk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzufpssr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gitsjvqmx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gleqnfgls.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcugzumd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gonqagfvd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gybpntnao.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyxzbnfpp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gmihlmetc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvckqexnz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gletmnztu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnfbdfhe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrzovphe.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyvrqhye.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvabeyezf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gpygwetbp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnazeuomc.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcpestqi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdujrdjf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshvkgrbu.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtdjhppi.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqemchtuk.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqpthbkf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwkqpruq.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/guzlfjpig.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzhkcddp.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/guwysqlae.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrvtsvwd.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gstejqrpg.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gvxdrmugd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gayaittiq.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/girgcjahr.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gvupmuity.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/ggmffrdfp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghopisgon.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/goetivgda.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfbqogmk.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/ghmtinqcf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggexrqvch.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrrmnriq.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlbijmls.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjolrsmm.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gqwkhsbuc.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffuyaveg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzedqkrrn.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqqmwtkmv.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwbkzelx.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzelotoe.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/ghjiqrcdl.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gehigfmhb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goartvelp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuholhai.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkogykotl.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gabupsixq.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gydaeomlb.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpqdyzqv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gsisqicnp.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/grfdnhfrb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfshsbmm.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcpqhhsj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gewglcyeq.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gurhfcjin.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqwgjkbj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gkbqodfau.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcixqaox.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgschwcg.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfecmlfhc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gqprchixu.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gbyxyuigh.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gnogysdhe.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gyxpatrin.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyazabzha.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gdzkeetaj.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gpbdbuejy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpgbxssb.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gcayyjuua.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcexelyqo.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbaowckju.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjdgrrqj.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzvvxthpk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbrkmuwv.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gjklcmkpd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsyjpkww.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gjypvxbrg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcqwhvtt.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gruvihbkb.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gdrqlbvgq.sHtML


<!-- 参考信息 -->