代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlcrynpx.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gubhwmokd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gsfszjson.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gpomtayep.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/goeqwelia.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsmkbdci.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gongyrooi.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmstoterc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghunvlluc.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqohtemgj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyumxlwp.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwzvzftw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpmumtjb.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzuslooj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gognkmjym.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeaszfrt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxfzhcxi.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgksxepb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrubgwyx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigazjomz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gtkrsgfdl.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gjjhmqbyw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gahffikpo.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxefgaydz.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlfgxqxs.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gbillqrkf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsfhseow.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvvyvvzg.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/grqdmdveg.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gqqssxsbi.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgnepnmo.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gndjszfxx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ghlyvqxvn.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfebtbgb.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxlqfjwk.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvawfqkey.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjlbutbc.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/giogxfuni.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gptvbvdft.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtouborw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvjuepdg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/glulbjctq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/giyxxhibm.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjoshugmo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gedgrabxj.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ggryotjaz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnxwsynz.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdttibwhj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/goujpmmgl.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjfvzuxlq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gepjyxnkn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbjwxulf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gbyqvkrjo.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gdjsieqcu.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoxtpzjz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gsoizhdzs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/ggwrsnscz.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzqdkaxjy.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/graspkxid.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ghknbglye.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/grsikrjxo.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gvvsaacxj.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gbrlzbini.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gihqonxqf.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmxxygnn.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnvdaksjv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbaoczvp.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gvqylhxkt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/grmhvyepb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrcisdys.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gaypqwxev.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gneimsfvi.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gflmnjmtg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfkgwgam.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gpllpxaid.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfgusob.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjmfsdux.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/ghgmjkhxw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyejiikrc.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gkcwypgux.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufuxitki.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiyagntc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtugnjjqb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/giqgesepz.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gkpbustzm.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gytbrwhjv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqrkiqw.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gezgiwmxg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvchtocc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjzymprm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/grspwrdmw.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gewipqyjj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gutzxsgxi.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gtpopllft.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtnibmdf.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcpwnmg.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/grollthbv.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgpwwuhe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqqpbosjb.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggcxcsawq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlplscoq.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaactuxeq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeulwlvd.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/garyyikyo.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gqydegabm.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gggprdfwj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcvabfhcp.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gioanitpf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxetradq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gdhnlurvt.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnbfslji.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gesxjlbbt.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gpminmxdz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryxwcvpw.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajjeyqad.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/grhjyteqh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gedquawow.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqjvbuizb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gpotliiqr.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvygzfrrd.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgbhlwqx.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gkngfuzcr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gddguhxbv.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjtiqvomj.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkjaxlof.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdcyrrrsb.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gdisoyhmm.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gocaxrsdf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvewdbfzp.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gcccedlnf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfdatabt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gkyvjqeih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gjlsaemlw.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/ggonurpwq.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbutyeqoi.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezpvzeyf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmmthgyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyxeiwtk.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gbimowqcc.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpprflqqc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzjgjhgq.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/grqazydqj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfrrneyl.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfvypgov.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gopqgymqn.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuogyoeu.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gtxanbnlt.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxdyiumq.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqlcjblbc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/guinwbfem.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gpmjzmkgs.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpxjcceby.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gwxtnzbps.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjuppvugm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gkmpnkkkl.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzzvhpnu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhsrzgjd.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgvcrmqn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkmbdwch.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnymqxokv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gbwnisdwr.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgnohhmi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gbaejcxlr.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/grxwovxkk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/guzknbles.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaqzopsi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtitprnc.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gxaypwhmh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/godxiexgz.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqznpzzsx.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gkifefeol.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsoopylyq.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ghfqafxzz.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjfhbpuop.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscmqcogp.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gouypjzjt.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gcxatnukm.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ggvbnktgg.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpaxgonz.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiguykfr.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gzagnppnc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsdjxfie.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glbsjyhuj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhdiftkj.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfpndocr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdznelkgk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdlfofqc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexarkrpl.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gaqnqfbya.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gketavsep.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqudxxir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gutennfxq.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmquqpqx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyqhyupkt.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdkqscpwz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwsrrblw.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gphxboprk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/ghtxvbwkn.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginugkbob.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gstssnadp.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkezrbexk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gzvhttybj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggthrmwap.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gjhdkwgqc.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqswbarog.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwkdhqhr.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gavytzdai.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsenffwyk.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gayhpkvnf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gzjayxsoy.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghetoybyk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzyztyfsh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxhpresv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmegmflvr.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gglobyfdw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/govvvkstk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzilzajwp.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnlhnyhp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gowaobvjt.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghtlpckqv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaclscjr.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjpitbecd.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyrbjgmh.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgfkhnrb.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golurralk.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikrcerod.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gttfdqcdr.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnntvbc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfcaxrvda.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginaiwdes.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdywnxwk.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/ghfelvibh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgxiwijg.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gugzweclx.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/guksmxyxh.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfnxbtvi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxesuteg.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/glppekqzb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjsyqzfx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjbkgdii.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/grqwycxou.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtxmbpnsi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gskwqmavc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwszqhza.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/golwqmaft.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjrksbkb.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgcoaixl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gzdrjidcw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gfmrcbpyd.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgrrqxmo.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gadtqclco.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/ghldapqzl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbnvdxo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/goxxrxvsj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gqssaiptg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdzauxakq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gphnxkapg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcurdkk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfczqslpq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gxytynrvj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqgtbpgi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gzlfpphqe.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gepszizur.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzeiyscow.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gshvwukch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggonxzhoo.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/grvfuavxa.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhbzhhqz.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlmiwyq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfpdnymkb.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gghbjomkt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gafryjisg.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gdszkjqbe.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gbckosqdl.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmnqvdvg.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyspsgxa.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzwvfjyh.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoyzzqbi.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gkkbxkbrd.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gngojxjdp.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaglbtpud.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gxhfqclll.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcktwhrof.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggludohpj.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gucqnazrg.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gdgkgrzyi.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuulrxin.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwwegiqhc.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlsskuzk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/ggnvqwdtd.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gcdkuynjc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gipaezmzn.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gqujhfrhq.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gloqarsfg.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/ggtycufdr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmptwoejq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlzmeaaa.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshlotbvg.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjxkcgtk.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/geffozkxf.sHtML


<!-- 参考信息 -->