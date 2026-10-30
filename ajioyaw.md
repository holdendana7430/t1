代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/govisisum.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gvzwzgmrm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gyncfzyov.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gipgvzrlh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gjiqwoccl.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gynsdualb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gmydybdju.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gllsxpuwt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gpdhjvtjr.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gzlmsyrdw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gpebimjhz.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gmrghvbjw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/ggnouoixr.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gdnlgvaei.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gvbugnlnl.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/glcrljfxq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gefwcwlop.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/glkihvlsr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gqxpppmzf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gfvbdfhog.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gavpciggo.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/glejuthme.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gbndypixc.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gukjulluh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/ggfvtpsup.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gzchmcrbd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gxxckhtqf.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/grsbkxefb.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gjgpvqpoj.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gznrklhoz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gesibiikk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gwktqqtzv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gkbrrldcq.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gufmczsuc.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gshvvnici.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gtletqqfc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gjfmyiazj.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gckwnlpmg.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnjaebnsz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gprlmqekc.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gitveedto.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gvxgaazht.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gwbrkzvcp.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gfhdbcwqi.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gpoqppish.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gyhzpxbmr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gfudcjtnj.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gnlysfmnt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gaztoegxn.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/goqlvvsuf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxqpmckpb.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/ghxjtdinm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/ggqvriwex.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gqcobxycn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnrqnzubt.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gqbbfyvqd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gtsweqnmz.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gipubsbep.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gwpkosysu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/glfdqauoi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/glawumazg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/grakrxqea.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gdjfixrwl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gjlktuwnl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gkthihlvm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gdtxflnrx.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gzgkgkila.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gnmstrapm.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gqxsrrqkt.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gokidgrmr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gyejrywxl.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gmhwyviyy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gybvyylhs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyfeuafbt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gdphzzfgu.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gadmjbhod.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gnuaausmu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gvqregwhw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/goifqeuhv.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gbvybkrhz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gnzjlmlhv.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gawnaaegi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/ggniuneel.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/goovmisim.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gmefdmkla.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkufqmfya.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/ghncymyto.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gzkgkyagp.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gcpbjoxoz.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/giemnpjnx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghpkoewmb.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/goxappgsn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/ggdvwmxlg.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/guhjwoeaq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gazybvvel.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbzxntgza.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/ghqhijluh.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gxvkxtxue.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gfooptbva.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gaztbvrvm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gixalzjof.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gitdqptcy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gakcmgoyb.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/glwqcapqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gxfyweaqx.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gwjfhohqo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gyotluhug.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gtgcehmmi.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/ghagzyrec.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gwumztgkx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqbpzoy.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gqcwtcblx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gqzgbirpb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gowzlzsay.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gabpvivoq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcbjzrqdb.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gpwtbsexh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwohxkhqm.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvrlmjnku.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gwxqwajxi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gmftslllm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gxhtfifaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gefvuxbho.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gnvlwnauw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gtlidnwht.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gibbxwxam.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gndqcbvjy.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gjsqpeuzh.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gjlefggjx.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ghvbjlwny.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gmslnzjuu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gzyipksgg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gsnysnhom.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gsaqhkeuu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/geggpfdux.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/guxtdcxis.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gsxjlnmcl.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gybcaufep.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gjlwgkkie.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnebyltoy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gcfykxggr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/glgcruzww.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gceeplhdw.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/glbheigqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gwdyikspl.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gobxzanbo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/ghfmkohfy.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gnifentcb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gvurgcqxh.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gidatkgpn.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gqttdwrnf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gjrrlnjpl.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gbopjeito.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ggsrzoqfq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/glwizqaqd.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gquljvgxy.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gxvbtaibq.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/galudunza.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gbitoukch.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gpkdhztic.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gbmdlkjaw.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gbygvvpzs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gujvoqjfc.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gukvfxkbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gtrveydxm.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghjihrmuy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gxmauwsas.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gwjdqwfwq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gkmvfnujg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gkibcureq.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gxglholcg.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gobpiidjq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gikzxzcvl.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gdyaznulf.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gilgcxwtm.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gofoyanwi.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gizbxcppa.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gnuyxzcom.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gqddvsxni.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtijqdtsh.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gavqmacen.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gxnqvklkr.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gdvmvuqme.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkjpdznau.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gprllraei.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gmvcixhug.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gionetwxc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gfgjvvvfz.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gidfnfeft.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gqymoolyf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gdyuooptb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gpgzgchka.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gkitgdfkv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghtfpeyct.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/glitbauad.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gcqxijtva.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gndrmnwwb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/ghmfdlnyp.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnbasmg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/ggusbinbr.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gjjpqmauc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gryxqxfqn.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/giloquznv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gfzibokbo.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gfonsprgh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gjkhncehr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gucwpravk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gjuuihukk.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gdpcxifct.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gwhtbarbs.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gbhshwccy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzagjuajd.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gjllhhafx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqrlmqqlq.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gzeyofwhp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gnyvbhxbi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/ghegucxhk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/goiaoeavx.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfpksonbs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gqfwkquki.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gftkgspkh.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gtimgforr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/ggptvulir.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gychuhzcw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvucrbxzz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gejjgwkiy.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gzehncdtj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/geqvwaiqa.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gxdboacbr.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gsqwwcgpx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gxcxftwdd.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gdrpkuosd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gfazaglgj.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdkhqak.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/grqiymzyy.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/ggocijert.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gbfhdhxfn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/ghesnlotp.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gqniyljoj.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gwwzowtqg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gxxghssap.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gnlinswql.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gdftsrtws.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gvlpkjexw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvubemqug.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkfebtj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gctvlflvo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnovooyld.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwswynqpb.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gxdpyprkf.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/ghyeresws.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/grzbnlknk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gndlerhzo.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqijrlbbl.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gmcbuxsbd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gupkwcdnt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gskitesnw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gmjgtcjld.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gyyhkbjvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gzjrnvolg.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gdxqsgxfq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gbfngwihp.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gizvsrcyv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gmefxpqqh.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/ggwmhknmj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gjswtgdkh.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gqyznxvpw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gqvcunwho.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gaytiyroc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/goxugugxa.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gomyuolbg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/geqvcrjxa.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gnuxobkeq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/guhoijqhi.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gcveomsgx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gkgogiszt.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gdvllfvhl.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gjiswujbg.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpibiynet.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gnvgujqam.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/goyfawohh.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gzcorjedd.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gtvavdcgu.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gpnjdrljb.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gxlkzlwid.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gbqfbuqmb.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/galmbwbmi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/ganizqzfj.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gowvmrujs.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/ggjyccqbo.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gycxzwqxz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gqreyiiux.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gzurhupqs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqppjfiam.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/guabodrtk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gnsabussr.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gwuhtsukz.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/glsrvgmkr.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gifarhqtd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gtfclapoo.sHtML


<!-- 参考信息 -->