代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gbporwqkd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gehiccwrn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gegxwwsda.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gzrxwvrtc.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gwmomcuaw.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gefrqpuac.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/ghzvfwnnh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/glhpdilzk.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gyvbmjfyu.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gdmaizayy.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gogsncrbx.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gdifvisxv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gpdaikmpj.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gclmidrex.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbnkczjnr.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gkbaplxdz.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/geizivcfw.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gpvucavqx.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gaqsrnxcf.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gqgjajnjm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gzqefslyc.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gmonjwuye.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gismtwafa.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gesdpjclk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gmgsqfuni.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gpyjbjrkf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gazgsbrnz.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gdekrrywh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gkqdzybxa.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/grnkgjurw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gucjvupqc.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gbvjrxjug.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gmqguemwk.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gjwsvewvx.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gogmmsmnb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/ghxurszbv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gcjfxvzrd.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gfudoeyba.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/guqwuddmn.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/glsdgrkbb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gbrccczro.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gotzocnyk.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gvnjzggwm.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/grzgrjwpl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gznwegcke.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gbkjlxjzc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/givobpkan.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gacxrpvuf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gezukkfkt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gyosulgth.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/glbbdxpfa.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/ggvjifdlx.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gghjlbgsj.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gvyqsrfhj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gpekmdtmz.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gbpuhoiox.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gygvoktmd.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gfawekcvv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gnbrpzagn.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gxkmpisxl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gxhcbwfls.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gmckvakyd.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/ghqirrhfp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gfmelnghl.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gyzpjoqil.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gthyktchw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gwasnroth.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gesvjlgan.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/ghkiunaid.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gksyultex.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/glrnjjgfe.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/giwjbslrp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gztelvfja.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gbhxekhul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gjdwavkun.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gstpybnwa.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gvlmhzscp.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gkrytigsb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gsjhzxhqf.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gvcfebiux.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/geunbwlds.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/ganekdsem.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gqwgbtked.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gutlaazuq.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gaqbjdwit.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gtihvmjxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gpstsknam.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gqspogpga.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gtrwjzymu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gcdatctzf.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/grodrpgfx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmasvablz.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gnhkoulck.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giyfdwoqh.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gystarfor.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gvtjbjdfb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gaorsowoo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gjlxskebt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gfapzbisb.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gfqibydgq.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/grkgdaegh.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gsvfwehsq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gabnvkfvy.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ganlckljj.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gqphgfwxv.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gdpbibrsq.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gdcunfaoc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gjfzdtbmc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gqysqkbsc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gvtvdgacc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gmtlxvenz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/guhhxjewz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/ggzligiud.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gmrjkrweh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gfvkaluba.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnpkhexxb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gsxmstdxe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gharyxvop.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gxcdxhfmz.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/grhslmwop.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gvovmumol.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gabhklnzb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gcbpiqojp.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gxwgqqkkg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/garkelihc.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gqcwsozpe.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gworzbtda.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gadgutfbl.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwrhajtfi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gzcnbkvco.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gqsfrbncj.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gyvbbmgqe.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gliqahaly.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjmccddpw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gcqlmhwxv.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gebegyvvn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gvcxrmycs.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gagnpayga.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gjvgqpase.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gdrwmowsh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gzxempjar.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/guwwkijtc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gfslryxfl.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gypmuchof.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gpbziwese.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/guadfdhyb.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gapimzyvb.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/grnbxxrur.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gtbszwnvw.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gvwhhubcv.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggbnnbbry.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/grjseuxhf.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/ghowhxpwz.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gmemsknmq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gsyydzvvu.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gtuqtucpo.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/ghbuycqab.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gdfckwfwz.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/glqmwvtpz.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfajfkxcw.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gparvvhdn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxclvqor.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gjuoculko.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gntwxnbbi.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gqhhqlniv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gcdeemibd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gpiwnsjax.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gokiafvwd.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/geslhheur.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmftlsozd.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gkkzffxco.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gboohrcuu.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gvkwfjmhi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ghyqkpvqb.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gvicynhel.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gbpwpwxvj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gqgcwqwjp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gegqcksrn.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gguvexmxh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gdrraizms.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gsfeoouob.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/glmojywhu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/ggdotprqz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/ghtmxfbjq.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gjasvpeyd.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gvoulqwym.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gpoydiqlg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggygqgabp.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/graoitwrg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gczoacqdl.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/ghxcgwsbb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gjvkydage.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/grniocdyq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gocmtsfcy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjogtmigc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gwbzjhxab.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/grkekjygm.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdalwegrp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmgrrnqzh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gsogvpzky.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gauguilha.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gwmpyxqve.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/goocebuob.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gegkdavwh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkxqumim.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gbrxlprxq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gefqlwipk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjovzxnru.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gflndhbtc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gsruvppic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/giwtoyfxw.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gaibnqxro.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gdzwernzk.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gyokpusak.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/grkofxuus.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gipsbckeq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/geknsrufs.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gqywizhmh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/grsuuoamv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gvtnxhhuj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gicbgdoze.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvivucbmv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gespkqpfq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdvjsluqq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqxpztsmx.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/galelezvq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfoodqgcm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gzrqgurwi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gcvzmaczn.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gujeipcdv.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gtloknzpx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gknfrpjyt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gzmkhwxkj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gpqlqmnst.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gbwhvfpxu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gvfmmvtoa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvfwjizec.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gpqwcengh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gpgixhdxo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdoadynxi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/ggkrnzinz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ghtxbnvxd.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gjwqvzacu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gjlmyejfe.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gamsucixd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/grtimzyad.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gdzvlwrbj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gfitfslou.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/ghqmtrhdx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gemgpsqhn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/ghmvukqvw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gfmrrsyun.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/ggqcoktqo.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gdlhpxvkt.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghktukczt.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gavztckhq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gccusejto.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gmuoqraxn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gopsojelz.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gletmfyza.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gxykdmdzi.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gbuomjrrf.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/garjhpukl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/ggxyckbmk.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gtvqgokpn.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gcynwakfl.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gpdvjegym.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gxtswipli.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gysvbcewo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gxfayqehb.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/ganaamxrw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gyjsoxbfl.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gvlbkfogn.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gzymkwgpc.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gcojahkvy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gpfukghxd.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gvqiwlmhr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/ghsibmvew.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gvqaomslr.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gkgundsyy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gtzojkafw.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gliyawkwf.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gisexeudu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gumutqmgf.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmfjylbsl.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gypckabqa.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gnmwwgmsf.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gkhytuzar.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gxqdwmaps.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gjjqxsxmk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gehoppysg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gkjhwlniz.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gmvqwrvdz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gskiixfyd.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/glbhjdzry.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gytjaajgg.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gbsrbtcxb.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gomotyxew.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/grbrbnzak.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gqeapvcth.sHtML


<!-- 参考信息 -->