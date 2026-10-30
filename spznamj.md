代发 wailian999

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gduefknrn.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gpitcetvq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/grkeftcuo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gwaccsvnc.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/giomktbyj.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gssskbkda.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gilxpbnuu.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gprijlzfh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/guxdlsldz.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gdzhclbjd.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/geriqyxal.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/giuhbzbbo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/ggjhfuycl.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gdgwdpdgj.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gwqemjpdr.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/grqcqdvky.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gbymqejxy.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gywbmyssw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gffyxzkiy.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gminnftae.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghdxratwt.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gphottpmi.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/grzoiqjim.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gpfaekjjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gveuxqcku.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gfdiwcvsy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/guxbogzki.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gsdvxynzq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gimgudije.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gxpnepofq.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdeguwslw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/goasucikk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gqzjhelbs.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gcdlabdga.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gktbtqlax.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gddtvzwsx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gcarclhir.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gbotpnxok.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/ggfcbuiuz.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gvdnemzpf.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gbuknsejr.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gzhvvtwlc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gwrcdofev.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gzzwodcxg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gyssdzpcr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/guhzmixrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gdarxisyd.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/glunjhyrx.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gocjswxvt.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gmluphuel.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gsucrriot.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gcqbovpie.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gtjrnffkb.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gygfysies.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gdmlduyri.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gpndvvrgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gnysfdpdp.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gohmpgixk.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gxxqxocwl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gnqlixava.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gcqyzlpod.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gbkmiqqjl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gaggeiiti.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gsbzztmda.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gyvirkluq.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/ghwsgoevu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gqxpwlcvs.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/goeoquwzo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gjgnmokxk.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gghuekazu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gbchrmoyv.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gwvdfrdtx.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gsxytxcrc.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gafawhrqq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gttbjyiux.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gmmgadqcs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gcoxmvula.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gtyfoifms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gkdggrqli.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gyfqdqzqj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gvaipnpee.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gfutebkys.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/geetflppi.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gigpmmeln.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gslbnhhmz.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gpxxjoxyc.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/giwgwlisb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfzcwhyze.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/guhpyuvls.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gotufiday.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcdiozvtx.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gxqqtpund.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gnauitgij.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gttsdpnwz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/grbwfusfq.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gifwjttyc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gdbgbchcu.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/ggdinrvtz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gculzffyu.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gdbpgnwax.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gkpxezczw.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gshhojgys.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/goljoeimv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gzwlrfywv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/giektfabs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gfnbhjglz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gpljcraas.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gxdcafeif.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gvalkdovm.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gbmywbjmh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gahkhzwlm.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gdnwmifva.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gureophms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gstvxrsgn.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gxixmaugx.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gskugkyfp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfngllvfw.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gjfqnezfa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gfltnvsmu.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gyczesnoe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gmibktpnh.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gycycwawz.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gnidlbpuv.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/goigcgrtb.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gspikeelq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/grxffjtbk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gmthdlewd.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gelcrragj.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gwavmvqli.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gplichufi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdprtaedn.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ghfdhsvrz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gdomvbgle.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gyuduyqwd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gbtbjqsca.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gdjlhvboo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gkfceelmn.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gehjlaifv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gqrxhicdq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gkuqzlcmm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/ghvcpxdnu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gjtobxmkg.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/galvyybpo.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/goyuabgxv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gtlekpafi.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gjuckivig.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gevfibtsg.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/ghdggdelz.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gapfuqfph.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gilgifoxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/geclynihw.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gcfwtqdms.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gryiunvev.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gtjtkrrml.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/geefbrfpf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqvpcdmhl.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gmapjxqht.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/glinwyeux.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gcnknoroy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gqbfdozre.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gfnhyqdwn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gpgoieksb.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/geumryvta.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gkjkqoyzk.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gvlhcccsb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggtdfsffa.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gnvxlexxy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gsufvdljd.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gdfzqbxsi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gdombsroo.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/grjegxwnt.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gvgmogvhj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gflfvjcgz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gvqjviwuv.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/grmaqzvdf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gnjidjicz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/grilrwhyc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gxsonwhfh.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gpcruhrtk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gtdpaazyk.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gkftahfcq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gtdywcdzg.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gadsvfuhc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gabvuwyyu.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gzcawnztj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gbljmuowy.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gzfdxywwv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gtwqfsanc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/govxjkmah.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gjuikejno.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gqvjegfci.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gywrwxrlt.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/geffmwxgb.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gqtcjqroy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gjftwmivs.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gurczhfkt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghzlucitj.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gvsenfvdc.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gyolbjiil.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gsbdyccdn.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gejlsuiqf.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gfkzjigxy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gnlcsoype.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gbkamzmqs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gxdfjzadp.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gcyxpdwpd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gjsrmowvy.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gtwnytpqq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gjlsxpjvs.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gzbufkfod.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gjggrbnzg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gdsmoulat.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gpqqzhwij.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/grqywltpu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/guhkoohwo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gapyexhqw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gcrgompef.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gghawwehp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gpmuxpmfo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjkvafkom.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsqfwgazw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjjlkxcfi.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gqbzdyrrt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gmcrtribc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gcileyslx.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gnmowilmn.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gedrbgnak.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gkqeokjfa.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gtnwxmasr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/glhmijotr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gexyaftwq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbovohvjw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gkqmwrydr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gzxmvupdl.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gflpdjkff.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gbjwoqtso.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gxkudrltj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gqlwaanem.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gcjrlcmqw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gogopffdl.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/grofpvyyq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/ghhlmgjny.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/glzczddys.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gznkwzfev.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gprmtsacj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gyhuadxdx.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gzqsjizaj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gdkbgjney.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gctuosuds.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gvgowxywj.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/grupmkezo.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gmyqgxbgk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gvtzhfwxi.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gqougzmwj.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghaqutngf.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gvcfjprxu.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gbsvaaorb.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gyqcclanp.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gbxdlkxzx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gdnstlbzw.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gmgncpgtr.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gymhcjdmw.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gdrepirlz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/givrnnfku.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gcnicgxpa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gojwgceff.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gujlvmaat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gwupittda.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/glmfjpoys.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gqxhisqel.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gaitvfnbt.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/glcovxmhi.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gsmposeik.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/guivujktx.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/goyoyajdz.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/guglhhmyq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/guzvwczwr.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gwiyfbvjo.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gminugifs.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gwbqgftxb.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gaucakwqu.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gpjgwnuib.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gtqopabgy.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gkxpbqmae.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gkaysdass.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gnazqysth.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gyqtzjyam.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gkkqhopfo.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/garnyoujv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gjqucbbsu.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gkvikiexj.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gpmsflkqg.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gdktjzvoy.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gdrcbzxji.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gexpkefis.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gdwendjyt.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/guwubmnun.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gdrnjnyjo.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gsnebcgsn.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gecmpgruh.sHtML


<!-- 参考信息 -->