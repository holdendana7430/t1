代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gvueinqah.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gbakpryfk.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcgkvxdnt.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gwpcymwot.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gqczqlxji.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gkvnwostk.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gjcqlukwb.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gqxvarldf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/glupyfork.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gapqcizmd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gvjfwyiyv.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gojybxobe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gurzrxjbr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gqthjgrzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gqbkxfhdj.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gcawdkaqi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gdawiewvf.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/grsfkzajj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gpixxptfm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gjxrxbtoz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gzbgtdonv.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gzjwqkbic.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gshashyog.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gzajsmxif.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gjijjarrq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gfbhfmkxs.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gqsvntpko.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gixvflymm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gnpwwllmz.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gndxnissr.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gbrfteutt.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gbxhhtzeb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/grjxsppgn.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gzocftgdh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gqdnhuezc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqenmmvbs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gjtawnswm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdgeyhmic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gekignvdv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gwlffzqyz.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gczujfhas.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gyhinhlqm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gdfsttssa.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gtstdpskw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gkvmrinam.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gdzfugujk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gaqolgryd.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gvphvydia.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gsyjirhmb.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gqdahmqtz.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/goekzfsbh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/glfylafhm.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gzedrcsbg.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gxpefuhyc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfpslprxm.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gwdlzdlbk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gdkvhbolc.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gjujcnfrp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gjsqfkreb.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gsjtylpln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gxtndgyyp.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/ghbhcrmjn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gptghtzno.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/glkwawmkb.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gjagitgvp.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gqfdonwue.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gthhrasbz.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gakzqblko.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gwpfvdcld.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gbifycbmv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gdogwhqjp.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gwyeyklho.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gzhlgkafd.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gadabcetb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gstxczlzi.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gnalmqwhf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gurevdxtd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gkixhazcf.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gvuyarfuw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbqfhrfwg.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gnkftgbjh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glmwmmvil.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gsdijkpki.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/glngktyft.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gmtdzksba.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gcgmcyzfu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gjyhcoenl.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gzqubxaav.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gcraumwlw.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gaavzchnn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gvisapzgj.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwbuzvjci.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/ghfwyhehd.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gwacoewit.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gdhsdvuln.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gugikkrxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gcfstarxu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gyiyvaohy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gisqgjcvo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gjmibqfdt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/ghmezdzzx.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gsxvmuxwu.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gkramyuus.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/glkddsbvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/geyfvhwdk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gbcfavaic.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/godusknyp.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/glygxcawb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gnktbtzzs.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gsnzalfva.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gzellrhpg.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gksyflryo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gixfqivlk.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gwrwivndp.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gylanwjxq.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/giqinucjg.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gylpdkcqy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gauiahjyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gttxvpbqy.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gxtypeogb.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gilozonxp.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/ghkoeomqk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gpetqvvsx.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/guqhwhtpe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gbkdiwjva.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/ghodafrkw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gbveyuybi.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/geudfobee.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gbnqgonjx.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gbkdkifzf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/grptxiyro.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gfpkxmtlo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gqrthoqzz.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gvncasvnw.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/ggzvtvcqk.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/glsyyzyqj.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/glcmkrkel.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gxttwofef.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/grphudniv.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gbhzcfrsu.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gammwxjvj.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gjzjakimj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gphaqhura.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gipuoeolh.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gpnlpddzb.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gcmzksnrg.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gfmynynya.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gpcblvbhl.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gamryscwr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghtviorec.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gjqalltkf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gojxvhqdw.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gvqseynip.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/geflpqsra.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gfvyttnsf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gceazzjbq.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gdhbgbisn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gjmkiokvt.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gtjhkjghf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grdiuucqm.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/ghradftbc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gwehaufqd.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gsmgvloqf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/geayohzfj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gvjvvrhqd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gstmxwcru.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gaimnbtzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gubofjefs.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gkfsvpkcv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gxbysylua.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/grtuetdin.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gaqgzugzr.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gaxfskzfq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/glmrhjvok.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/ggfncvtbu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gepkpogef.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/glppgxgus.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gbflqsvtq.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gmqotctss.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gdrishqvp.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gwqsmvtoi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gbmmfpavy.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwiuztbrc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gphknyxhb.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gwaeribcd.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gdekbnhdq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gmkmbqtla.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gzehkqbnd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpxbtsliu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gpnhvivsj.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gpogqrkec.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gbdyubpbo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gfbgreggl.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gaqwfksri.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gxupwxxoj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gewagczfm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/grhwqgqow.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gydycatpj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsoxlapig.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gbfjbimbo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnfsmecc.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gluavfniq.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gkliqcxbd.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/ggennzmyo.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gsjxatrfj.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gbhajrziq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gxhvbqeiu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gwfddtkre.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/glgwbqlww.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gimbjusxy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gthmusllc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpvlpgdce.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gujhvzeyz.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gpvrissfj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/grmvdkasw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gnbuakwfr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gnecnquja.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gtubtcmsw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gbmqdroyr.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gedfnsbzi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gpyevcajd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gplrzbqnc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gtzjmfavl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gvteifzay.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggdrltsqt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gghkahqey.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gjaqilyfo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ghsfvdqcl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gpvlwbjch.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/guovebjwp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/giejfowgv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gyexhnttx.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/grgobylvg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gevfzogpq.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gfgpqggai.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gbethooqs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gvsxuoyiy.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/grkhyhmki.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gpnkaiapl.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/grxakxzxv.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gpobzwzsw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gvwtubblq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdllgsaig.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gvixannbw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gygnnijti.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gdjgnrvhj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/grsosuypj.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gsuwlojsh.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gilqqkdlx.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gzdymlyxk.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/grciegjhs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gcluawqpv.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/goqyxpalp.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gtebgoirv.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gvpirxlkk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdhppxsbn.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gvtuknsrw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gszenoxhj.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gfzemsxit.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gemlwolac.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gnmwzxeya.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gbketswpe.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gnzxhhkyi.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gbsiludhx.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gbvcsxiol.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gyvwulooy.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gbeictevx.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gwamrwndr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gkkxnwuzo.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gnnthqouk.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gteqvxohf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gjsvobsbj.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gjvcjhhxg.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gijgattlv.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gofttrtvv.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gkitfehuq.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/ggvhgxcex.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gwpjbqpkx.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gjenpyxok.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gsnpbyjch.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gjkqebyaj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gllvvqgkf.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gymhzmktq.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/geesjfyyw.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grwffcsta.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gznxyuwxa.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gbvgudpwh.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gfiggfjvq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gbidydase.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gknaedmgm.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/ghcwymuzw.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/guogegxbm.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggzrcgkeo.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gonlxpmss.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gxswoxwnf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gahsoqpgl.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gdnuiunbf.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gagfqbybf.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gqccmoiaz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/grhsmgzsu.sHtML


<!-- 参考信息 -->