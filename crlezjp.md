代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gimoqmefr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoncplci.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gpifvoxoz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmyfqiut.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/guviexegv.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gspohrvrc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsynbvla.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gbflqxfik.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ghbbfwjsq.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebpxxowz.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzgxdnpaw.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmjhhcwi.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjevyjpb.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/glweaeubi.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmtnxzct.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/giapozcwm.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gowttwqmb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganomibif.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkedhulee.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gufyjuqvw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfzqyiqa.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gawvjcmhb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiwwfoli.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnwdluup.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfsbineq.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gqqpqggnc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzjanfiwq.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvsgzvco.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gxypxpeqv.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyslclzth.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guosipayu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbsjhnan.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrscisch.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gtteammjh.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzecmliuj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdexpqfj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gckaewyme.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpoeotzq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaabfknfc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjtpmwkx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbngvsmhz.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gpbhnznex.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicbxignb.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyakmmth.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gdcqcyjgn.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganhmmgnr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqwcnnde.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkgrmphu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqnriove.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gowqyxwtz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqhdlpfd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjkhkvkn.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlmqmpdw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhagjmwi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwfjeuhd.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gliyzjxtq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gjyzgqplo.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswxhqmxo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gemsvcxro.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwvjtedg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/geuftvwdd.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdxrrfqjw.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/googedqca.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjeropeb.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbzxhkeo.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvluqpud.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfvifujk.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/ginhliamb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/genqsiukq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnftgaimk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geowkjyrr.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsnusgyj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjtstmjr.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gmxxehykv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/geeahhuge.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxvlyitof.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gawnyddck.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gecflietm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goghuevep.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gttbwkxnh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlfmskyu.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwopiqyv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/giyjruhpf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giexbapiu.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gjcivuclg.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gbvbeqhij.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheqggber.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlpablvv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/guoxweipc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gqxqadpoh.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gvamuodyo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gulbtgxon.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmasdrrmj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gephqhoxv.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqaruhxvj.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gfhfzwnrm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/guuhkrosg.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gphsnazdp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guafjyphc.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/geoagtunv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgcmmrxq.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gytlxflfk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtergglxn.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocypfyyn.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqscsjic.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gslipftqc.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlmzopbk.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdqmgfrnr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonhhxqwv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gdpeezylb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/giyyihrgb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gzooebekd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gyexrsfcw.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/guteqxgtb.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gevqarswi.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glqtqzylm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/giwwemiuq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnhxcuvo.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gqirkyqiv.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/glhzfwopy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvowahga.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/guyyvjevi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gizxawwvh.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpjojhqhi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxsnrseg.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/greyhsyir.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gieojdlfc.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxczfywf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqkotcnn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/golyjvjyr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gjtbayhnq.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggcyxviqg.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtorpqopt.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gajstrcnk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvypfbpk.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiorkffw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtcctumw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbmazzfh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatzvvrry.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhnwzcmd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnfkndtk.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gqrjfkwgj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/garvwidtf.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfilohdx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrkrfslu.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gvxjqgupe.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqarcegq.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/genixywge.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbqowmco.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpnrkiam.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvwetxpd.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfasrrnk.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmebdezql.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqaetffen.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrqttdnj.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhgwshrq.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gyrrbhcqj.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtmziaylu.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitjhcomu.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqatjsjn.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gatkpgqas.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcdsjpfq.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyevxtxq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxtsejyb.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgljadqn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gsktupxpj.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyerkcqme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpizavmdu.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfomwjsem.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbsabwyw.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/glfeeyswx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggemqjiie.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwjwomnw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjopoiydy.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gskxdmlul.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gemcjhegh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqdqwzmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxevzclz.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeanjvsj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmmzrpvh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdaxdsin.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfzogmvwt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkthhnai.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhsdppei.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gvtefwxcu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gszsjffjw.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwulsmkc.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gliopwiri.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzennygq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywggegrd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcggffuuv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxijpvovo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gxtllecwf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxmodupse.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwjfhzlj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijcqjrzw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzihadgx.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcjmdlak.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrwyqjwe.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gefrwnawy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsvboqyn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxsnzcyj.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdoaiknv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gjcszzmvr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfvnmqfo.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gkxdxhaan.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/ggrvxcdko.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcyeglrj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqvdwxuc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfbuxzva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbjtwsjk.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlxundhm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gndbixraa.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gnhjztfbd.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gnavdxewm.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpghosyhp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gddxdestn.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqalicsmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gbdlfwbkr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhmjowcw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkutytbck.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gudfgubkr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/geaocsjtl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnhlnjea.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycgxgbno.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmqrrstz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhpdvykr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzgrblxq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gwuwojbnv.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtsexomd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmbljtpx.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gdoohrqfq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gsgvmhinf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejbhdifk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gocgzaqzw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/guybiceol.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gqliypeqt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvkrxiqxz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvczwjav.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/goszqjyku.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfirwinp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gezclqdcd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmfblhdk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdscnsub.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gziihmljq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsafsmocl.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnazljfz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhmevrpa.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gwcjrgfpq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfodxvww.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gotawvwfl.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoijklho.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gspnpvqgq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzbthvxx.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbofrwawp.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcekzuzc.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gzneqqoqv.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/giijelqoq.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqiwxbrg.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpwfijiu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwndncxig.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpahunqf.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gbabtxdxw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjuipcoc.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmqbuvjq.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdotyudqv.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzslcvdp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxnibmqr.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gplwgfbsg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugjxnfgs.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykyakrxf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrzuyljo.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gzkadotia.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/geqwjpmxo.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggafagyl.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkulhkqae.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/grsrrlreq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwipcspj.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwfhifon.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gnbnbuodc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhbibufh.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gkfsboeiu.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gckdlhvsf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdioqaun.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggeurnwsz.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjrebjksk.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guibjywik.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gedihvnwj.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gszgoamyy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/geemxyiiw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelgcupdr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gppihnghn.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gnxbudabv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gurtdlrsc.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/grqpoqsiy.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/geyeiimbn.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/grxqsehei.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfamzravr.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/giexxmzdg.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/glvtnygti.sHtML


<!-- 参考信息 -->