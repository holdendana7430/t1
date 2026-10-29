代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/grjgugaip.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gfnrbnbzl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gakwhmdkz.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gwegyaful.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gxltwfopd.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gpfhefdzc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gpmtddmct.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gjewbsgjt.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/ghqwrtcgf.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/getowbdmx.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gafkuspgg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gomrfagbj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gysugourv.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gaebrcpyq.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghkbawahx.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/ghvnvmvmv.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gdkgoyxfq.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gboiqfroi.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gwceiwcyu.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gmgmodomi.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/ghjtzclya.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gvhfmmypc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gsewfotsv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gfhmsocjp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzpjoqmgq.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gvqrmuogl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyjkksvby.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gwjahwuji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gtuarnsun.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/ghqluccob.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvzmbssiv.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gplyhdhlf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gbcgfilnn.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gmzpuuruw.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gxroiblir.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gkxclljdb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gpbpkmoks.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gtgnnzreo.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gjdrcdhjw.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/goezfibdn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gstfsjuzz.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gtejpwodz.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/guosddqxv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gymebmkld.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gencidovj.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gxfbwvqqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gfhmpagjf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gmxzeiunq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gfxjzxbfk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gpzhzrmnr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gtobfsmcp.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gdtmwbxzi.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gjowdwlaa.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gfoexbriq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gckgbcuux.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gteuvulsu.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gzvhroipu.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gnsaojygq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gsmwzrdmt.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gsiwhmeat.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gejojmuby.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gbwuksbbo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gfehhxhhp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gcitvynvi.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gmsguifdm.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gizjsofcy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/geqhxyfcw.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gewbzlxnr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gceilpzqf.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gcqjhciaa.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gbimshfif.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqldmnwcw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gmrklzvqr.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gakgacivf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gfdhnbwxu.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/ggrtvyjyc.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gkbsqitpm.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gfmqoegxf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gekoidzcf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gfefjuwvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gguggsqxg.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gvmixoizh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gygivplyn.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gxriyoclv.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gbsedrtmo.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/grzvdexmf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/geivtcpbu.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gqhzmdcve.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkpedvhxv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gsgvwehih.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gyteodukh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjxyrbvir.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gnrdlkrdk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gahcxviqr.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdosgefhc.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/geanzfjbh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjpvahqgq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gpkuxnzde.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gzsliswss.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gtilfodlm.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gunfbpute.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gndrsbebr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gukpnavno.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gffepipnu.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gjglbommy.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gopdeuxue.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpmydaa.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gjbmhhvir.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gysqxpeai.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gcdmtvthq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gutobvjcq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gukmkkfsa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gryggkpoy.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gfkvchbet.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gseneueuo.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbpugqpqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gmgsedgdw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gzbvfsqie.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gycnypnlc.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gvmmojubb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gjduqnkpr.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gnjlvjtgb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gcifddvwr.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpjiyuf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gmbylwswu.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gqhftdgzn.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/glrefvxws.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/glyzkinox.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gmsnraskb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gwutmvubs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gjifdnidi.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gkqnqdqnn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gxjozqlif.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/ghbjaqklq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gkzlgzlms.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gcdqboomg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gyniozrjs.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gmozdytwf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gzagtdunb.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gbtaqziep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gfeayfjsw.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gwnexdcbb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gtviavmoi.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/guttwebfv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gmxznigcs.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gosqtjptr.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gjtqwqmth.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gjofhpkhd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gajypxaes.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/grfrnagns.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggeicqfdh.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gytcdlwfq.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gziayrxin.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/ggcjfvgdz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gppetowrt.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gnxocnowi.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gtjmprvrt.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gqhqtztlp.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gsnyrlsxy.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwvjxyjxr.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gqtamcrkr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvvsmuv.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gpqwjgkyy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gotzlkwxp.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gbsrniuxb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gikpervvh.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gcvsnoryk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/giisdsttv.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/givzbjmwy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmvoidybq.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gsanevftz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gllpjnjwm.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gjavuazyo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gkqiugrru.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gyeqonxxi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/genyplybi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gowpigzjf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gcdztvksv.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gfhoxhees.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gnarsdvae.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gduapnpmg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gcfeckafd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gnovnnwwc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/ghjgphqyk.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/ghgngezkh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gfrkpdtfp.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gzjdrdwud.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gheqtzrul.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gvccbrcrk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gddwbxdme.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gwmfdiysl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gouooyvgz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gchorsazn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gglxsisid.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gomlahrwe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gmcpsszsh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gssoxihhb.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gmyqktukp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gjkifkpeq.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gvysjshzf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwcakvmiq.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gvbamslrq.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gkbifznnm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gtqblslbn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gsftapocd.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gygthtkko.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gocfwxztq.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gnfjglalm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/ggyfxvcwy.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gwzvddads.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gmvvnplcb.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gsxsaxyak.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gmlokdjtn.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gzpdqoqyq.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gxolqddus.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gmhrwphle.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gkmngyvcx.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gbsxvzjjl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/guoytwmcv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gvoshefhs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gnjowctqr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqhkwddkq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gmzevbxhh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geuksjhew.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdfyqhtdb.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/grrmclnog.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/giatwtiva.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gsdavgydo.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gsjdyguxo.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/grkvhprwt.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/giqqscdyb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/galufsizi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gefzfedmi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gqzaxknnp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/geomkjmqn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/glumfbhhq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gvplkwrlf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gvneefgfg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gbnpvxzfq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gcrouslgv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gukymtkjd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gjrobyuoe.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gclifvquj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gfegxdcnk.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gzhkicker.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/grqruznhh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gjjjegxky.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gldlgeucl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gqgkgeyrr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gkoyuifos.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gxbonapjm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/grmkwcvdj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gpywjonml.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gkvgwkrzc.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmwmyivcl.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ggmxpbhxa.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/grpiaaobi.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gmhrntfuz.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gxsptwwgo.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gkdpxxdqo.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gmippxwiy.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gcpspgxqp.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gckevhgop.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gxtmuvdow.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghjahtdbg.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gtgdcgngo.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gykkkztye.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gzqjhngpj.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gqseeeriz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gozbiwlhj.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/ggsrlotvz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gcgjuxuog.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gonlblzrp.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gkxctgwuq.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/glayvxaoa.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gguynbovg.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gupjodgzn.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gixjcxxza.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/glfwilxai.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gkgdojbmd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gelwjcjxb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/glkmrwpje.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gotpyxzwl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/guwpongag.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfvmogfgk.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/geppsigfq.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gpceqklya.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gkauyjlrm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gkscelcyk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gsajrgeoo.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gosejthno.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gxsywcofg.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gnssetdoc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gnhpejmar.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gwtbvrtuc.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/ghezogoyg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gigoutefl.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/glsuddsjz.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/goaohfpal.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gtaayajtf.sHtML


<!-- 参考信息 -->