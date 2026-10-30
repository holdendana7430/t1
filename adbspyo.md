代发 wailian999

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gkfnntsnc.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/guablaizs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gfxypylsd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/galmbhssj.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gjttfajkb.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/giwtzmhau.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/guvxxmfmy.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gdlkbhpus.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gnzipvqmd.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gccvqhtnb.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gyecfyuqx.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/guadzuifu.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gpdennclh.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gorulhefm.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gpnkgovth.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/geqcgnonl.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gtzkdoitc.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/giqsmbehf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gvvaxudiy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gofikzvkh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/grtkhbtao.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/grkizcuzi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gtnnplalz.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gaehszsoi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gwrklcatp.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gootdmidx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gnkugbigb.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gojlynjse.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gevgcveic.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gbswejooy.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbdswapai.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gfvpbavpg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gztpcrktd.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gewoceqty.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gkvjcqzmy.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/guyzbagck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gstnzswfe.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gsjhgdufz.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/grxnnhrct.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gmqsnwnax.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gwymvbgrd.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gfcidqzhj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gkhcrkwxl.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gxlunndlb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gvegvosik.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gsjjiptof.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gwtssocgk.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gaizrgvrb.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/grnuzgqox.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gayytwndr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gxmsurglm.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gzkzhgbwt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gqdhkcvqz.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gfgulkdug.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/ggfcwkuuy.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/grhbwkywj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/ghsbmkmzb.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gwbxikopk.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gcorcbcvo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gmtwbhdzh.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gagckdlpz.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gexpdrcxw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/ggtcfkeaa.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gxtkfrcjt.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gawwcxdcn.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/glclxujvy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gxfdcrxqb.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/ggzvivafe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gjpjkcolu.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gphzlisqp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gfcjsdjqw.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gejmktngn.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gjjkfjcee.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/ghzanbgjb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gcxynqwyo.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gqmtkndwq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gbhzzpztw.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gdeqtvkws.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gyamctort.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ghktquflc.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gkffulxhi.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gemuwxdun.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gmvmwqbep.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gejhenvmo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/glcqwcjfk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gbsmcralp.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gufzqwxri.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtdapaolg.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gnvvystys.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkjpavtzy.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqqhgpdeu.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gisrnbliu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjldlozg.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/guxlcbncx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/glrmqqfsr.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gpjmqmcji.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/grzqmdrms.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrsvich.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gsmnmywkt.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/ggekrhspx.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gqagifcmv.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/guuiizytd.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gszsotlow.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gbsmvmhws.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gvnjipfpb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gzwgpumkc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/ggycpsjbe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gaiwavute.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gfobuznud.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gcdfnvzfo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gtkhevgkn.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/grovjobop.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/ggopbcijo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/grrxjqshj.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gugsbiaih.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gumavidmy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gvqrmxvgt.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gewnfuzyu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gcnzkgeow.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gkrbwhryx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gmbkzjpzi.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gcopjfwds.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gdtwluuxq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gqjwqouep.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gwagpfykp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gdvblrfrm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gljftvuux.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gsnannogd.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gerelcxoj.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gtlyrofjq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzhnqgvvi.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gomgftmrc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gecsohhhk.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gtqtgmmis.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gocwwbzoc.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/giztspofx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gqhojrlfz.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gulvvxwkp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/giatpjymu.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gkqjgoace.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gbnqtwqbh.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/guenacaac.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gldeotzza.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gfqrfrzwy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gixmqrdxo.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gmnmptgis.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glwezksix.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/grflrnfue.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gfuzxpdjw.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gansazyde.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gayjbqrsi.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gqdqdvsnx.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gwenxebhs.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gfxfbovov.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gmqxculqz.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gutixvexg.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gwkznarjq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gavipgrhl.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmwphyxzx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gmomgrplz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gbwwgggxe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gwblecqzo.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gxwalfwox.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gqitvhhvr.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gnqmhkrbw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glwgjbnhz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gaesmkqsa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjfeiaqbk.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gmzwogyuq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gnlefzrym.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gsebhvsfu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/glmqctpfz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gzdvwqtjr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/guoojqemd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/ghqdlcbpo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvoofizid.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gzugkvomi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gwaoauemm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/glyhhpxzj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gnmbqyntl.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/givndsffr.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gwvwxydln.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gsqfuowuk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/giqptotdm.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gjhgtiqzj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gerroydlu.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gcvjcipvt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gofzfluwr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gkjmqvtgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gotutmoev.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gzmewnesx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gxdjjfucj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gaformrxt.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/glbsjsroq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gqkwerque.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gtocbzcrw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwcwljtjj.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/goqskdapk.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gtdonxsvh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gzmeazljx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gnbjbhrug.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/geposhfyi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gltplpfsr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtfroqqih.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/goubejzfz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gvteafkyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gpwvtclvj.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/goqhjurej.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gfcygrhff.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gzpinqalp.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gugwjzoyq.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gpykwuvyn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gzhnohtrs.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gfatewvlj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gpskmmtzg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gvhmugrie.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gifkbmddc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggbuvqebi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gbxyedhhk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnujtwkzt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfpzmggpd.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gyuadarbl.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gxnwycxhr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gyvqmptqr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/guzgfrwhc.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gncxkcdsi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gwkmmijmz.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gsesuryeo.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gnqivehky.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/garolxmmx.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gswfbdntg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gmqblrssl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gsfampfwe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gcstaaklw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gdmjjunhv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gqzviippn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gbttcocce.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gqsyfkajm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gkmdeivwu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gwwbqviuc.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gwjoiopzi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gchrmjinn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gpojhkfll.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gndwibien.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gxhfmgwti.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gjheeltfn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gmxxdqwfj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gmrjgkfpn.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gvcyznghk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gguzmuoqv.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzqdqjrzo.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gopryoojf.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gdzqeunwu.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gmxnjegzg.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gllhtphix.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gxuqmymwm.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gmarnoprh.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/giwknigzp.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gdzsvvdbt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gaglqsffx.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gmyjcqwqp.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gpdvlbcri.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gpfklsfvk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gqzxegxcu.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gcsychhqq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gbkurpzsk.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gjirnuhia.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpbmleaq.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gkxxkyspf.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gbmdijkcw.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gwgtbvddf.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gfljamzvw.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gcwaxyhze.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gjyigptin.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gqiurpvuo.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gpfuzrvhw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/ghphdluwp.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gktkcqyms.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gaqdyiutk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gasphfwzy.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gflfpgzlp.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gopkavphy.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gtmvmwxoi.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gghiecdhy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gjsbllrvl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gmzybihug.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gekfzkyou.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gxnlnjzxy.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/guunvhlci.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gyemeejtr.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gzltklklb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gpikspech.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gieycotjn.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gztkdqzng.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gdfgmiuxc.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/goxautisr.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gzlyfzejb.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gyhrfqdsx.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/ghqqiknvx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gpmwnfxxa.sHtML


<!-- 参考信息 -->