代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/glhgafici.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gftbjbffy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gtfogjrni.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gmmzhtswp.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/grgmpetjy.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gtzmhqjbt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gbbrnjmnc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/grxqbcnmc.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gztzqazio.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gmjfzjetj.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gfzruesde.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gsvlxkjrz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gzqmwvglv.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gcaiffdhc.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/guuaaowpf.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gusakakld.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gvbiqynqn.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gxiomlcra.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/grshrglib.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gpniegmhb.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gbwgflxsa.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gzzgiihyv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gseeprxjk.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/ghdixzmrj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gznrgxnbb.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gfraaxyut.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gorzxzxxj.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gzrrpulbq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gcxtvcwsr.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gojmqscay.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/giscvcrca.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gplqilfux.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gwllwzlka.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gzklntshk.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gibjqzmwh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gofomynhu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gfqjsmpzh.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gilojfhur.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/giytualfk.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gujwcyair.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gudjsqscu.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gzdlmaczv.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/ghrgckobq.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gfmvixpwj.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gosaojpro.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gtvrbdobw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gohvjwzrp.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gmpjnyrot.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/ggsulwhva.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gcowraxjd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gxjcktxcw.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gxuodazhy.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzadbpzic.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gwdasvtry.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gzcxsatbk.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gqgtrmoub.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/ghrovqurd.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gerhlbpuy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gnmztmedp.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gczxcyxcf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gwxloimll.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gzutoqvzk.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gsckepuhf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gltxxlxju.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gucsxlrqp.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gioeatveu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gkfpofrka.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/grpvnhevc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gdeuitshx.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gtmsaimcy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gonsnewoi.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gcpvdipae.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gyzhseoax.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/grnewujyj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gminfzmoc.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gejhjpehv.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gnnljbouq.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gdifcyvds.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/glpwaazgh.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjjjqsvua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gndbenkve.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/ghgevnnrj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gvzdgviny.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gmgjkfmcv.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gtmcotbid.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gpgaglxdw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/geukhvfha.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gwwethmox.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/glaayrkvc.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gsempyiyj.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gbydfjlkw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmtmawviq.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/ggjzteyer.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glgqenssf.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwvegntip.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/geidlnayr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gpjvtftdz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/grlhysifo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/ghlbvomnl.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gyrcdqulg.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gdzkagrfz.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gaivdfqnq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gfujhxatz.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gwxslgeqr.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gsivgtxwn.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gtrixlbhf.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gdbdwkgcr.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/grwewrumn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gunloncgg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gzbvsaftb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/ghtiqjqjw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gzofyfwkj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gowggnaue.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gcmyynmsc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gdqwtrekw.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gnkoqzswl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/ganbdgfxm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gekpefjiy.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gqmjtifis.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gvftjtrdr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gclsfbkns.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gxyzohxyv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gjmahrzov.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gkghjzemi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gcmcmuiwf.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gkfuletmy.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/galauxxgh.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/guxhxqgzp.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxxzlmp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvdecpbrb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gbxecedqv.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gtqqmawng.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/giwxbdxcd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gwhqddbwq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gmgygvciy.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gwvodrged.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghmxdabuw.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gcxruywfh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/guvkczfic.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gdoxohkds.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gtqtakgow.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gftjuraev.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gukruekxs.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gmfjvchcx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gnvlbelmn.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gyodhprkk.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gjjaiwbzv.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/giznfmmdx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/glidmngyl.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gfbqxtiwl.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwkblsbxy.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gcdbbhrqm.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gldhhtbnt.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gxctqouja.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gmxymtcoh.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gzxbaidev.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/grkbnmkwc.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gjrioisob.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gudgqahyx.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyqbasgbg.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/ghjigddzs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gwsiudrrm.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gvozuoajx.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gskddnxto.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gbyypxldk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gngesjwpg.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvyvpurjp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gjjghgcik.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/ggrjzallg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gieeisvys.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gazvxkapq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/guuunptjo.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gdebyulaj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/ggabireho.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gdmtwnyja.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gvuyqwpyg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gwivsvwqe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gxuzykmks.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gagdifowh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gagbmebwc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/ggjtvxmmb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gmdaizpjj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gaozdprqx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/guybonkxk.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gitwvsotl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gpsxvghza.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gfgtpgnaz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/griensnvf.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ggjlyeifo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/geypccgjn.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gnifmuhak.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gawkorydi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/glyyagmet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gtwhtpyah.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmwldzrxe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gtnbozyvu.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gcgifpgcd.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gzcgaclhk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/ghhmhtrtt.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/glmtdhyos.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gijmbwcdt.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gtfjudqip.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gklfjcuyv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gaahblvjm.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gitikdghf.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gbcmvyhca.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gtlflhzvt.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gxgiizwrt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gtvjkamvr.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gjbqyqhkf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gfcuxnhfb.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gmhetplks.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/guhjilmyf.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gzptmlzjw.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gljmvelmp.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gofooxhzj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gusxwihxr.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gahchwapd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gxqomurhc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/giwwcqrmj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gswbdduua.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcpwjbtbg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gyouscsch.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggmqnybvq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvsaauuoz.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gzczjuirm.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gpijpvghv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gdokxehvo.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/garbxzuwf.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/garfostqx.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gwnaflrqk.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gxhqjjesp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gxwaimzga.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gdftsvprr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gxaaoolsh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gsqymtpfn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghyklajoe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gzqlxfvwn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ggqwvwwvv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gzbrgphba.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gvjatvuvk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gyknyludc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gubcvmcbl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gtpifhktg.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/geyneswcs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/glgmtyflw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gwnboauqa.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/ghzymqkrg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gxqchxuyn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/ghrjftdrs.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/glijnmjft.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/glwutrwjd.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gmvtcxins.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/glydkpqhu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdmglcukd.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gshmivpar.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gtolywbvv.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gmhilzjdg.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gseklcjrx.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gtahtvdrj.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gkufprrna.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/ggudlcwno.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gepokwfoj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gargpyyhn.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gmqilcewx.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/grheaieex.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gpevrqiwm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gdmahayuo.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gyhhhaqkm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gkqptwzre.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gvbnfhpdf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gnkrzjxah.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gzegdebtc.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gtcsdmoel.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gtyooexvc.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/ggrzmezkd.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gixwzwglx.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gbkwwqnje.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/glbhfwmps.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gheywsmdd.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gduaayhzy.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gjukqrlli.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/ggizyobjr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gttfftexh.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggnrmyuok.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gdftavzkx.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/ghslewifc.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gsczbhzsr.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gfhuzthsp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gfqyrtayo.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gohzqiomf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gahzeymfn.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gongdcvmy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gfkqbqdrz.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gzlestuip.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gzzttvrwx.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gukjsdymj.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gftfkkyrl.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gnqkhszjb.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gkqfmnroz.sHtML


<!-- 参考信息 -->