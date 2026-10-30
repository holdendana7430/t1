代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gchharooa.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gjmltdrdb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyrtspdhw.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/glfcqlluv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnisxasz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxnjvhna.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gplmjhedh.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzrgsmj.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqayrclds.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gbzjxpdyd.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdxypjrcj.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gimhmphey.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzdldrqrc.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghjqqlosr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gynwemvcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gkplgchtx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcmqdafob.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gywtodjkh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjekugwio.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gboxybgzi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdpfyoxc.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gslufffnr.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gnytazrjz.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/giflybdjh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnequceo.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjujlsym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjkafbi.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrafrpmc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshwjvmmj.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gzozgkxbm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqnxyirkp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvopumwlc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gsawsfsdu.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gftjiuoqz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gifhfpkzp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypznkhva.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcudpleyc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gutlszvlk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzwfcshv.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwvfnongi.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdyziqudj.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmarvppyw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxazzivd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gezxisqpw.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkizstqdn.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsitjpoj.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glhvajnya.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gaivcxocb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdfamtzvt.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdjgdvsk.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giztfjogs.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhijklrg.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gktrspmby.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlksgtvy.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gwialkboa.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqpfcvtv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gdbxbybay.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gmowbbspm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvymgokpe.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzznnswe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giatlrtnu.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuzjybip.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcdfllkto.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmovwbwyx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gzzibutgh.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/guooswbii.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdxrgxvcs.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdhbuxgq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbcklync.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gigwysnkj.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gezcyrlxw.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gccvnqeid.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gaynbiync.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdiwyqsl.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoquytfq.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gxshygtyi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gszgnoqct.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gbbhzresu.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gumulgteq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqwgnnt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/girdxpckp.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyscprwwc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndfngzqv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvpgbpzl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfugwtcr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqbbxvst.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gtyhowcsr.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyhrdgce.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvbpdbmw.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gozbsabvd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpavppm.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gmczneusb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnycipql.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gwvediciu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwumplwao.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhfslykw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnfugbfy.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/graujsovu.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gotlirbts.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnbskelv.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiopgfen.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfdbaaod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnctstbdx.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjfrgaju.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrbscvd.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/glsubvsoj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/grbowqfwu.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfktpezq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gclpzfzfh.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gvigzizil.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glvtivxpx.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gebvlniym.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gbgnyaged.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/glexfrbec.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnzswdxyk.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmlmuqph.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gbsdjslex.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefewtrfr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/goqnnbxey.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gbwspxiuy.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gysuoqwzw.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnohhhze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpooykwsf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpalbsyn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwdqpinti.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcykdbau.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwyazlbu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gymsfpjnk.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gnugphiwb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnykziiuu.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gczduqoew.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gbcjpngot.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdnbicmnz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnlqvjhg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxoonrua.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzwaftp.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gedqjzrdm.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/givwxwrgb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgadpryo.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxadsczgm.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkxmveat.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtvokvmut.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/getlrkzlw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ghkspkadx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gcxginole.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhcensuy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypnegrmo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gysvwiqxm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gyovnihga.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcrkzhoo.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gadkvbtnn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadywabbc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcqenyfb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcyaadku.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxysvkmv.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuzugpqg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpjzshtvj.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gfyhdonhy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gezfjngso.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxckqmtnw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjbdhuos.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrectvtr.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gskmftera.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gssaivezk.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gobuigrgb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/giwtqkzoh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnvlkitl.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkypfqac.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucwiiqka.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjrlqwjsa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbldnmbnr.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtsjzded.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gbjtcpthz.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gabwunueh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijrfivnn.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gerbhptmt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmbmhas.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/guinmkgfm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/guilgbnpl.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpbvtjdz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gughphjmb.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/guutwqcef.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqatidek.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gszmelvvr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmtsjtewd.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhlhmddj.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwkdojxqw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glomzbvtf.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfdyspau.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmpniabpy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gohilblzz.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gpcrotmds.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnbgxbgu.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeckefbd.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gaczuwemj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbubkeiy.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnbzsble.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjnltuq.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gtjcqpfnz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkbtlhla.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/goomksdbm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/glmvgiacl.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gttnsmbes.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmixydmhh.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gygqumhlp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagsvucca.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gsmwjvyqp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glmwnpkeg.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsyhurzz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiqaadmk.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guardnfgp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrpsmcmp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyepemlt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyfwnezl.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gwepjjuse.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsttqpuni.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghgrnjsxv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/glkbjzoml.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyrxtyrf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcnvotwn.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gikrzvlww.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvyuqtgg.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gqduucuwo.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdycfbwf.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbipouate.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golcsgmey.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/glxlkbkfv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbqyyoxyn.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gdffdoxlt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvtjliuj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhafegkm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/guiiebwcc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexuaswiy.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzslbdtv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdphxoyq.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzqfrtc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcxnhwjm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrdfzcnk.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/glstzgtrz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbhirusz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggywvsdnb.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gcttvdyjc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gezzxanmh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmqxguty.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcylbgag.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gekyykdsq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnxhrpbo.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqdqtrsz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtijsiliz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppawxgfg.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigldtap.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gheaskgto.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gteqvewuj.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gqhpfhkbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdstlrnbd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/ggwqecjmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxrbtnfa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grrxaizna.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbxkpmlg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcygcsgxn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gganaawsu.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gldjmqwcx.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gewskcvpj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gswzovpdv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiweskbn.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfsuybvl.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gqnffnhgb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfricvaua.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtienwves.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwbkdulf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbipziwwg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpubjtxr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmkvkskeu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjqzsjbd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkfteawt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/goeadinly.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gleqyfpsb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gniwrfhrn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngkrtdks.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gruywbboq.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gmthcjqch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfvknecv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueinfaud.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooerrtqg.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gbxzovuvd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnshcgtl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdjdktms.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcinkruoc.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gtgaslxiv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gybkzfzqh.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggadqbwwp.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/glwykfrlg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxeohxve.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grlxdheqi.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gwvzeugam.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcgyeqtq.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gxfhxkqfv.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdvzhzljm.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gecmluzui.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfezzmji.sHtML


<!-- 参考信息 -->