代发 wailian999

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gmmighgff.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gecdjmjab.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gosvwawcr.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/guzlammjf.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gkahoqosg.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/giybprngl.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gkhhlggkt.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gjnuezpgj.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gnvgmqwtp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gucofctdc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gayraxkwb.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gaghjnhbb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/ghpbwsctx.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gawitzfyv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwnkrslfa.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gbacmwfsc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gihtcihzg.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gaeeimdoj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gdlevjpjv.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/grmylqgte.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gnvnyrmbu.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/grjgilgvu.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcyriifej.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gnbladuss.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gludgyhdi.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/glzzrgbsh.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gifarlotf.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/grfmbtwev.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gfpmunllm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gbirsmgpq.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/godulntxq.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gphkndvkz.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gwsuvkygb.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gunyikzvo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gdcsrxwif.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gceqbykyt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gswgbdnpd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gjqkpooro.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gjoispvsv.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gbiggabla.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gwqacoond.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gcskugpji.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gafgdtmbw.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gmvndjelc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/ggbshnapd.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gdqvnorwl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gtzgfrkvt.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gssrytghb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/geydyewer.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gxpktbfbs.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gpjycuvng.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/ggjfgurtg.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/grbjzpker.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gjwwrdtkb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gojqpswmm.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gzreovlwz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gzkeagwqm.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gyccifxpe.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gkqxfnigy.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gizsdkrjw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gryoilylm.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gpvpngzmt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gpocigwhq.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gtvrlnfwx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gtgcydjdf.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gdwvxdalg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gwsdovoej.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/giubbtkzc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gsswyvxwo.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gkqyoicgh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/growykmnp.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gvbqbycbm.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gkonvmywb.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gakzfurcx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gtjxezvma.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gnrxdavpi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gjemhzsob.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gideigejn.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gulttodfx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfoypkouc.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gyorglhbq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkzihvhdi.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbwbxpmjh.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gnsqeoctd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gkpfxouje.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/glxzbxgas.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/genagbgou.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gzndljesa.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/guqwwwuvg.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gjrscqlgd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/guvfcdreq.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gvamtzznk.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gorgstqpm.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gfxyjopon.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gphjxhmol.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gaddoyuky.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gjuvhdcbh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gbsrstlpa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grkdabcfh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gvkguckfv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gsasumvmn.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gothapnsx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gclqhbmiw.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwxwvumen.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gaiqohimf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gfjjnkoeh.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gwaoxmqfe.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gdzzqblsf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gcaeftopv.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gavgvragx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gniqhivzi.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gtfvjkuop.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gyrlusflu.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/glfqxyemf.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/goygcplbq.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/goykzghfl.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/guocgjqmj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gxxkccffk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/ggoluqdbl.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gyfawmksl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gpkjlvqqz.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gwfpbuekn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gkkgoqern.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gtsuzfrdn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gpeufapdy.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gpxfsmtuu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gegbxgiuk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gvctqsovp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gsqjjbeis.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gvkgqihpe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gbeoljyis.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gthvbkezn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gjchrjznm.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gypdhdakx.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ginnlolog.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gocoflcsi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gdzxscqal.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gfzhsfffd.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxjoqrjxe.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gbdwfiqpd.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/genaeryms.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/grkhpqbyv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/goihofkgh.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/ggbwbgpzc.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gwvfqdnhy.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gabwipvty.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gtfnirteh.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gspjhbgdo.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gcpbwbgnq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkywflbw.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdxitqkja.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/goufjdccc.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gxvmprdut.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/grrwsqtpl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gskguhmlw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gwjgyqxni.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gluknmuuk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gasruxptv.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gepooylzd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guldtawci.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/ggwrkioan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gquobtifd.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gsakzhzku.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gtlzboopb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/ggtpachdh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gvemcjyna.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gemktjxlu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gnmdspbxh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/getwjjizb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gvrfzlglp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gzhkjorls.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gahltqidt.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gsttjsozw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/ggxuftarr.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gikucefed.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gwedrdyys.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gugqtuwyy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gfjhhfjbx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gmonibnvg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gcjwmdbhz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxkqmgsme.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gfgfbgodd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/grkacapzn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gfybxdzzi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gxunqcivs.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gcnflzgra.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gyjymikcs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gdmomblhh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gnplkueer.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/ghjoprbgk.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gkabwgizd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gszurzzus.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gqfzmhpok.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gahintxkj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/glwmmkhut.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gjqsxiybw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gvhrkgdmc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gpibaackb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/glofjbumd.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gedtdqxum.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/ggyydbdmp.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/grtxphzeh.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gwddpvgsn.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gomnesnkf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/genlzukbn.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gasglnuwd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gwxysxoxh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gudlnpvax.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjdvkazoz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gprfhtmrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gyzbthigb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goxdsuflk.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glwepsist.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gskiriwdg.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gvftvcagz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gpxlaitdd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/glfzinjkq.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gighyypwf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gtxixgoum.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/giilkyzda.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gobfehotm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gbtyyhqng.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ggwiwvifa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gcminiitk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvtondgdu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gwusarydb.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/ghoqbcmaf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gkgnrzmos.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gfpafwzji.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gkcdmdwrz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gbnmgkmqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gpssgdjqj.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gkxiairlf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/ghsnhggtb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gxydxdvkj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjhqwqwti.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gbqintowg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gsyuzfxuw.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gylefbjke.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gplkemqer.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gyznfzgkw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/ggnvngwns.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gxuiifpbh.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gyaurgpte.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gqxjpolgu.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/ghbtxttgo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ggiedsnny.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gmwyhpbhi.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gjvqcpxvq.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gnbdncmaq.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/glfvvanbw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gqkrdxmfh.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gcdsvljqa.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gltochjsp.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/ghcmtqhnd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gysfbyzlj.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/grjmcmdul.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/ghsquxeiu.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gggdroptf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/grfrkysbm.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/grnooficx.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gioovblbr.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gqfdydkhb.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gtrlkslnn.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gnvuzpoop.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgnsvhnw.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gzfcbxxfz.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/guupcwpsm.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gkfquaalk.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/golcpofqp.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/galswulun.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gfwlzezsd.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gutgzldty.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gmeodhzgj.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gefzvctuz.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gkffwqgks.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gmvovwtus.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gjkumqual.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gdfsijffu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gtmvwymry.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gjxqjlonn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gvakcuglb.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gsalemyul.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gniqcqyew.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gtujvogtu.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gxjrzfivz.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gazpcxtqy.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gzbagxkab.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/glkwftvnk.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gqmesgsgq.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gismmmqxr.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/goszytddi.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmxxajszf.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfffxkmfa.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gxjspzpcf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gqwfmezfc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcigzndgh.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/galxtypds.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/giycfkiyq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gqamteazk.sHtML


<!-- 参考信息 -->