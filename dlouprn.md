代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gyzehthki.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gbfamfpeu.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gehvybtsq.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/guzbmqoff.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gbftkaubm.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gzgbfmoiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gqzbweebn.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gxazhxult.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gubdkywza.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/guuhadekf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gisymveus.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gjtfgyeym.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gagadcjlo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gbrvqenwi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gonqqjcbg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/grfjmqfzt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gelcbhpol.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gceohgrgj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gkvywignu.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gviurwheq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/ggfzhempb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gufcjjtvp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/glcpkstsx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gfgkwnlqm.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gddmuktxg.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gudaivzlp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gugfdbsmz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gcvpmsvwa.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gwbipfmer.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/guezulwvc.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/grwtzevsa.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gmvsikold.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gtpjjxepe.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gcfpldzhj.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gfygfnudb.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gpktnzmqh.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gkvepfizi.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gqrerpktl.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gfovnnprl.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gknwkkcuh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/ggrikfisf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gcobkzyjg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gnaejnfjk.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gnhivecrm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gkdefbgib.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gturrbmwa.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gavksuids.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gqeoklyzj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/guzighluk.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gzucaxeqo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gbkuvvyrr.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gumutirhm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gabltookw.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/ghaqahike.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjziqkkpp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gwqdhtkzw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gjmhrohdt.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/geeksmujm.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gflyteijd.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/goiaakvws.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/guaqtxnbx.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gabhydwmg.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gykcsqmku.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gxcnawlav.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gqproqakp.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gtpqzjknz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gfhforngi.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/glvstzyyn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gihpsivdt.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gdlgyfhpk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gvpftfvis.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gklhjzaoz.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gmjnpnmkr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/glbfyafzv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gjykcwact.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gwmwidbdq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gfezgtjot.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gcljsravl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gdfgbmjyq.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gujzoahlw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gukykquvh.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gnykzpzoz.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gwoyitazd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gnaedsvxw.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gqibbjnwa.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gzlaovrts.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gyswcmyei.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbttsbn.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/ghzextkaj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/glqlvbtjo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gcxdaxmih.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gyadklwwl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/germrdkbb.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gtlqgqwcr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gcghowaiy.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gllxgluly.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gtlnrbiqm.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gmdzbqxmp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfultlzpn.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggggjbidr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/glpwmmvgl.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gmupgffxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gsskgovpk.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gryyyfvxd.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gsxrigyws.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/ggsvlpsgn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gpwbplnnh.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gmwyumiaf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gnmfgtmpc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gtzigolzw.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gecyqkrvx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbbjwcsnu.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/ggmgnvgyw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzmnnookl.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbyodszjc.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gwqipxnwq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/ghzwplthf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gabbnegfk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gyzhllrsg.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gyskrckel.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gvadmxenb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gpbscxhub.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gmhlfytyc.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gprtbwtfy.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gdcsxxbbr.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gfhilktrx.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gcrxoqglj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/geiopdvsr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gwzbeimur.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/ggcynlsde.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gevekkfii.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gnuycarid.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/guhvneang.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gtjnhxecs.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/grghdxrik.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdpzvdlpc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gidvcexsb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gsdamqrug.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/giilifqwb.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/goniefzhb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/glxptwavk.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gyvmbjuoi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/glaxokkrj.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/ggmmmfrmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gjzpzbmbi.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gpkpoiafq.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/ggkcpapmi.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gwpkaarup.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gphqtlycg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gceozknhb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gyraidkfb.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gclooqwdg.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gnlzzuzky.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gowhkjcdt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gjudizjzp.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gsespujvp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/giowluypq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyhsuej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gtzqnbyed.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/geqojjaas.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gqrxumvct.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gxhhcoekv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gkofccepp.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gwsiolpsu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gpztqykce.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gkyytobip.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gpaleeyvu.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gxzignhub.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ghdigmlxo.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gkxlyewlg.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gcflqsooz.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gniqlpbua.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gopbbvhpy.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gcqleykun.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gauobstjd.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gjxnpjjqy.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gisjxmnqp.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gwnzoegsi.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gjvgmijkr.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtukcpkep.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gycsmvprk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gwhpsqttx.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gyekwwhua.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gizjhlxaw.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gtqlepdez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqiqbtfwa.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gdcodtkub.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gzxersjqv.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gtydcagfb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvszzlwmm.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/goxpnapci.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxqtxnwrt.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gdhzlecji.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gjraoafdu.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gaauobgcs.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gzcpivkmu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gcdvdstev.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gotkfdade.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gajrpgfpq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gtddxkhtu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gqittonmw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gctyslhih.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gghxvgwlo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gjnzsjgut.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gnqqemglv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gawfevqns.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/giiutqfji.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gyxdqhpjb.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/ghejnbles.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/ghiyjxtcv.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/ghhzvxfuz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gfugoplhs.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/ghzrgzmzh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gfwijbxcn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmsqgfgeh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gkwnoiqsu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gespxvhtx.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gponiglbf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gvondaxol.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gcpjsjrol.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwwszltdl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/glockwsgj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/ghnxqkwhd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gbfkactnx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gyteaoktd.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/grzlyjzcv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gjaaoydel.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/ghnkgoxia.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gqaaefxrr.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gogzcldzc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/ggxaansmy.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gxechxxsu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gabykqouo.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gjsntolrk.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/ggjbrjymz.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/genpizumc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gsjcpowjb.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gaacacqjv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gaeynmzlq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gthnxvwnj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gtasbgpxo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpspjbgtq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gcrlxbgtm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyfpibbxf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfrggsrek.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gfhcvuowf.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gnuqivmtz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gesaraarz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gjukuhidk.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gwmqnjduk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gylnkksis.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gdtyxatzj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gebuyigwh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/ggtjwonru.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gmhnzfnjl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gjzutvzuq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gqcwbghtr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gjzybtjge.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gozrbkwuf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gbtbmhppb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gilrawwfk.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gproqzlab.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gsfemokvz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gcnixwlub.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gvubacdpf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gtkebngsy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gybcighuj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gyfmhyahq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gbkacybrr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gremqtofh.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gttmzzwlv.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gijvnbavn.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gqpnfghni.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbwnwph.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbbgrrfst.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gzyugxtxt.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gdhnfuypp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gsegwmxmw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gqqwyfccy.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gowazgeht.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/ggcgpwupy.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/guckkewhh.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/grwnduqji.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/ghwsnevgo.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gqtrkmwlu.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gbgywvfbw.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gqpphjhhh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gznzpztkz.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gvxsqmjkh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/ghxsdslmn.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gqktohxpy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gelzsvgad.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/glxxfbtwt.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gkdamlwqi.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gccqpwlln.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gvxaemyxc.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gmlggpade.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gjnxijxmx.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gedglljgs.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/grdeeixin.sHtML


<!-- 参考信息 -->