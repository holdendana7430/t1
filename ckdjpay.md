代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gpzzsooyq.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gkjbnczjd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gxlsmkkej.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gbsvkqqft.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gtravmutu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gkrkyojdy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gbksakaia.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gwcbfwnay.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gceuljjky.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gzvnyphlq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gkgueapdf.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gmmkupeyw.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gamgbhjem.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gcrsshocq.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gsryehdon.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gtlnirfzf.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gcdcenefe.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gwseswobb.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gozzhdavh.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gkpjozthd.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gjufhhgbo.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gsnnbwssc.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/ghzlzpuof.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gqkipmxna.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gjgnezhzp.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gbsapektl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gijcfklqt.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gdrawxhet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gjhjqymhp.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/grpxtbvdu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gahmsseiq.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/getuzewqh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gpcjozklj.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gjljubaic.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gctdjngdk.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/grjncjtxe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/giefntcht.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/guiwfqqxr.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gzkpcggdu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/grrcctuev.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gcmyydymk.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gzsbedfxd.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/ggxrkokqu.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/geryotgkw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gxuhddgyh.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gpibzrjdw.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gpohrpmpf.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gqcnboros.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gcxiqxahe.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gonsidjtw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/glmgnhvac.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gdwkjdvhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gjyfkcyqq.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gyiropyxo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/ghnpbtkmm.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/grgpchooi.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gmxvqphgv.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ghionsnma.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gmlqdhhdz.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ggeuciayy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/glgiamjhv.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/goklcjjkx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gvqzqnkal.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gtcfyispz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/ggozwyswp.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gmficynna.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gmtcxuejk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gfjhccvml.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/glsfmvruz.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gwskvjtyn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfnnlaehb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gyquqhcbd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gezfreppp.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gjzendxfy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/ganhhkuir.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gchxbouwm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gesvhzrrf.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gzrabkkwj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gfpuujbap.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gcodaofol.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gcggzpzxs.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gjgeyhzjr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/grsedfkmq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gzqmizhik.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gqxassjqf.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gpoqtrena.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gmooksnls.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/guukdadce.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gevyyatyj.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/ggjpadwzg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gmxnmuiqs.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gftnerjrt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gbchbgixh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gootttnsi.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gswkaryym.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geipivapg.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gnxmybjaa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gklbpcqex.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gldcfrtnp.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gdtyrrtzz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gydifcvcl.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gsejrfgdw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gjjawelwi.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gjkqupnzp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/godjihqws.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gmqigoxwp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/ganxyzznz.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gmxzgbdbp.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gietlbidb.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gzshnwzlt.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gkjjhtwxn.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gtsxqston.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gernoaxnj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/guhmpcwij.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gwtjmkqmp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gesowfbqy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gcqnvkccb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/grbbtopuk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/grqqaohba.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gasaliaci.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gfjfmzkur.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbwvokzpi.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/ginkmivhh.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gvkauoatx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gyiezcdfs.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/ghnjbbygy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gpjyyogzv.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gotibzhdm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gfsljatox.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gtczislye.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gufpeoupi.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gjtrreset.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtxiumxot.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gowocjjpq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gmhnmthuf.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/goivyoneq.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/grrxxbtya.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gckpexcqi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gndmngbhj.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gnoowbsqu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ghutkixmc.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gfryegvoz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gvymzkutu.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gbpoudmsi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmfbzuw.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gwrjycthe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gpttiijfg.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gmnpbkalh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gyryrxusl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gnpuzfqot.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/guchlgavv.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gflzgprrl.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ghxjilssh.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gyfuqefex.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfxrfnqdx.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gsrksjafy.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gmothfjue.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gnnphmmng.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gesfgjloi.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gjaqutdpl.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpnknyjsg.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gcxmaycpp.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gpjuedipm.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxzwzynmc.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gqfuaksrl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gpcsnrycy.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gzgtafobf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gubbjpkic.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gwenuthoh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gevejmygz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gldtlnkdc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ghhdglftm.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gfztagabk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbeqtdeis.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gglhnzaed.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzladlytg.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gpnoouvgm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/ghcyuqsgs.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gxbjazmpw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gagescypk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gpgxtnsnl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gjzwbvqps.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gezfdephk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gtmjqelil.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gyybgasht.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gmuyainig.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gijayemsu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gigingvku.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/ggokcwvxc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gmrcbbbao.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gmwqazuru.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gxqijkfhj.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gearwlajf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gaioqewbj.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gqxmtslef.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gupdlkwdf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gwwwbwbhn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gjongzozd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/getdoizys.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/glfztooxd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gndztjqhp.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/ggkywrnvh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gsyzcnxsg.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gilrwdhhq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gozmgqukg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gbeykxoim.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gktqqddyu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gxxuwvrhy.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/grsbhyprb.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gmypxcokg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gzcatftzj.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gecaxuysx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gapleuygb.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gunjwhvgq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gkssfebov.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gnexhkwmk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/ghcvhrvby.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gemhefvqo.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/ghjcylpql.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gnkuddaib.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/ghjofthnj.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/glrixnwvc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gdmwgfxsy.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gaqnweqma.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gdaugsqim.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grhocpulf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbyczdywi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geegzidsc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbwzaqfiq.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gnhnbgfjb.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ghfbzqbtm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gxingbbmq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gesiitdaa.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/golncskjp.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/graggxtlo.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/ginnhtavv.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gfhprklvl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gmfbwnkyd.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gdnddgnlt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjcfempgj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gobnjstes.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gmejuxqxx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gwqyvnfjq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gikyqvupw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/ggvnccmfu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gayauuije.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gydyfacui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gijuqyudf.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gjgtlwjdl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gqepwhtxc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gilrloxik.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gskrtkwnw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/grguisybu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gfpjlfdng.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gtpwymtpg.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/ghqerxshb.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gpkkvkszj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/goeuwnafv.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gunknvqlr.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ggazalkcq.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/golcnebnq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/glqzgblky.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtikttvoo.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/grtlhtgck.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gvxldzggt.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gmwuyrjaq.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/grxegfqcr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gbazbhrzv.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gvlsrqmzw.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gepugcthg.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/ggahdytku.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gfoxiedjc.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/ghurugohe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gslmziitr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gqkushuki.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gtnquuqkh.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/glwpqkvqq.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gysjcdfpf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gunobcggh.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gexawehrq.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gqponjelm.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gpucldrdt.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gaghpkdlb.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gfoabewfd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gignkqymq.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gerfapaxg.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gfdqzsomp.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gutiqvmzc.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqtziihfj.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gcgupnyei.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gsxvfaxsb.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gywpxoote.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gclwxuede.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gwlogmuqn.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gbryaafzy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/glvrakcoc.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gwqttftck.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gtuwrymwu.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/ggrpmacxz.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gnmwsdjpq.sHtML


<!-- 参考信息 -->