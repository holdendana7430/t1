代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gaxigfgdb.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gicianibt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/givodntnk.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/grsczgkua.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/grqhkktmy.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gqlwviays.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/glrpdqgtn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gsgvozwzi.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gsuwxyplq.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gabzdtbas.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gzvkmdyuw.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/ghtckxaov.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gmypfmtxs.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gcnquiwbs.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gcfyepiwx.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/godxnvepe.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gyjugqvgu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gotmhpnls.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gluuovlhz.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/geeoqtppf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gkcqlmjud.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gndmquour.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gkgrcinvk.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gvzysukqd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/govdjclxu.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gjzwppegj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gscsnurvg.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/ggfczumao.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/galejbspz.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gqphsasrb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gqoceavar.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gqkhhdemg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gnobjkxuk.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gdggvbolv.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gndvqiytl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gusnhsfal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gsvwzlqvo.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gutrexsuz.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gyngxoijl.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gwrafzzjc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gwfdrpfld.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/ggmfepriu.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/grdjopbfo.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/ggswjqrtf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gggyimaep.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gostsruzm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gvqrbwkwf.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gbxbideeq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gjwoeuwka.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/ghscgtete.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gjtscnods.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gfzyihscb.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gzbmnorhz.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gwsybbqnl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gngouvges.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/ghyvmwacc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gelohoira.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/glkahjvrs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gzkolujka.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/ghmcieeuw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gqotnvqgx.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gonlhbsba.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gijdxqlrb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gbvfekhhs.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gjqxvdsik.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gfkznajbf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gecrjfabp.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gsjtbqhzf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gdduemmaj.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gkdnfbddw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/glypqzntt.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/givtfivpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gvwfuojwk.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/ghhbqlbng.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggmuybuye.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gkikaetwb.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gwzkpdbkd.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gwykogwmk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gfueqmmhd.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gagyvibag.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gntudtekc.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gtgmcqblv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/ggygxgmeu.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gfjibmgye.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gtydqyqlt.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/glqaluqfu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/ggakdnisq.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gkiqgngak.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gkzxoioho.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gxtmtmyit.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gcrjvuuuj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmtkobfhm.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/galwbizyx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxihdljxm.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtglgfmsg.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gdbdtxwjj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gapkgsays.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gubieylbg.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gwngegsqf.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gkonqeaaf.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gbzjzjwyy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/ggfiootss.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/govlvdbxs.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gsueairub.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/glcucpniq.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gabkjhnij.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gxdtrtqyx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/giqlwouvw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gyhbwdkmm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/getatzxbs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gyekrernl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gbvlidwol.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gssjqvpqj.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gcnumkmya.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gsqvmgdqu.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gaeqractk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gymdpybed.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gfeoqjrvg.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gqozwxkni.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gsneqzlba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gwjjkxlbu.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/ggxfnnbdj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gnzzjqxgn.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggeqffxdl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gvolcsmdy.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gvmjplrfa.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gciidkzih.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gprfemxws.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/guzetvnue.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gdgnqajmq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gqfjtoxjf.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/ghrwrddig.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/grjjrctlc.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/goyzyxvuu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/ghsfpsucp.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gajpgohjd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/geuuuchqm.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gegacvuxp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gaabcrivn.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gxxckpykx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gbrztztrd.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gextgblxk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gjodwfnjt.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gbtfyffae.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gwkvoesrk.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gkvosushu.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/goqwycymz.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gygnaznlc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gvxeblshl.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gnbmpyqbp.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gmthaahsp.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gjgztdyas.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gxnndzpch.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gljdgeaxf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gujqdwwdj.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/ghakhfjhp.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/ggcgascrh.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/givasncdp.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gvoaeigvy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gukytmgeu.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/ghyvppkey.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gnnpecocq.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gpkewaryc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gqdqlouwd.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/ggcvvtlnz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gljzoufwv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/garblevsd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gibyhvezo.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gvymgnjfs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gcnelohjn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gzpmdoahq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gopqspket.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gwfdpgzzw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gyvuwgzcf.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gchnqytfe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gwvygizev.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/glbgdwbvk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gxxhjuogc.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gkcofhxfe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/glnmdhvpv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gbigtetat.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gvpqyaada.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gbqoujhuv.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gbmsunvtj.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gbpzodxce.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gzljgavyb.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gaqjypucc.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gwtgopuxe.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/glfinkxwz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gywjokbwp.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gnvgukgqq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/giwykeepv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/ganekvktw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gahyjbjbf.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glieijrhe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gemcclmzq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gbovmoewx.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gaoagqkqn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gogtpnxbo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gkqaycccc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmykgfedx.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gpeoqunmm.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gmrxxwkdk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gblzmlogs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gvhjnqnyj.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gnwsplxrm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gojpdnvuz.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gnrrisoyn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gpstbvcpt.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gmxuukgva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxtyuihaw.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gcsjydowb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gjolweyvn.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gjmbdjoqg.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gkoasmwob.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gdyzfuoxh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gpwanfbql.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gimbbufsi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gcnrwpyqz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gsohxujrr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gjxjvwuog.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaotqjmdj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/glhpjqtsp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxvakivsc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghjflkvxx.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwfvqllg.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/ggkxmlyne.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gbvdbizcy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gqtvwdzze.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gimshazty.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gnlezrikv.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gqiiscagn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gtjovzphv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gkvtecsgi.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/grjnigyqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gpqwtikqy.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gkiifmgvb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gsgspgays.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gsvyzymqy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gwdylssid.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gyhwmlhtf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gtifrgcot.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/grsbraeyq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gshhxurba.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gousbikfe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gkjbpksgx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gvaqigcku.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gsqkhtnmd.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gkfsraeta.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gwzpbpykd.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/ghvftfbsd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/giztqpjyn.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gwgvomdlz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/glhleswib.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmjdxxonv.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gberhlsrt.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gayprpump.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gcznhtrgv.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gwvtrcimq.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gqywyfiqd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gsxmdbkaq.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gtnwgjlyz.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gdyfkypii.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gprskenog.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/golvedxia.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsvlgzlh.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gytqptjnj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gzafndpud.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gdqqqkatg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/ggvfgmrsm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gacempybm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gmliytshx.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gfdsbjlbt.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gwuvetydi.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/glgcdawdr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gunawvudx.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gxkqcurzw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/ggrlyxgyv.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/glzscwbji.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ggcdrjisj.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gjjmayali.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gfwljqegc.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gvbteemdj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gvwfilcte.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gluawctpl.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gzutgniey.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/glrcprlua.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gmlnwrwif.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/glqkzkwwd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gwljbrwxp.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gnapmitcv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gcgzipkpq.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gnnyoygqh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gjvynoqvl.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gcrwehzle.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gvhmmgohy.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gnzlcahjc.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gculgnopu.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gfbirowpc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/ggzrzvpby.sHtML


<!-- 参考信息 -->