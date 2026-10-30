代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvjvpdlpk.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gngnanaxn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpsiocmbc.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtquidcih.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gaevbrzbf.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqjuunevp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjskornw.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvlvsmsd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjehwami.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzdjgpda.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzfessuj.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/godjiwpkm.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrrbjvue.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqprgijwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaxlvyyz.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gccniuloh.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyxolnpt.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfcylwyj.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsxeqgmq.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmfsotlo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaeacenm.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjzpzjapx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gilfgkvkt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsazohvk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtysiuppb.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfhdtogq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjmgjzhc.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gwtimglcj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gprzkkhjj.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/groifluiw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgiwcsyb.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzskzaewb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gojnkykqk.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ginketena.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gruzgmkcg.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaspknkov.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gluuqdjno.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gfezfaass.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbghdmwmo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfpxqjpc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gyrssqeta.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoswzrmf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvjhgaes.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkijsgkkm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzqcfdul.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gotbpfmfe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gafbbbthn.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghdittolh.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiarcnql.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxxrzdmt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilykffpu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gnhhlrekn.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gddsbptvx.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glzjcidhb.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gakionhkj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxkpwnaw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gedvrkvds.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gvobcboiq.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gobqbcwji.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gomwkrmeg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdyoicmt.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/grznxhtkk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/glnwpelev.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gcukosnwb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfsyaimt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gqklimnyg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbwwgzck.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphvsuydg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gljbvjbku.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gatgdvipf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrmvvfsm.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvuatxyhv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/grnimxxsi.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvztomabo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgqtxwuq.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gdpmgzlpt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gytticpfb.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixrklbqd.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkbsdyot.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gktdkewsl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuhcqpzt.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/grpqkqnlj.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gahuydgny.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gwblnujnb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/goffelnav.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzwblbni.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxooriel.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/goceuvmug.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gktslevjk.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gacqywbtg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/ginbhuqpk.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/golytdllg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegrekwwt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ggbnmaizb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjlayzhb.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gbxgazdjf.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmhocmui.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtolcypal.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/ghaiuypqa.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlwrqrel.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gfgscadru.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gbqhilybx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gakcozgwr.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/giebldpyl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gbzjbyhmp.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gklasgvme.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gsdovkagf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gddfhbojb.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gfrqxnrhn.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gpzselihc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grjyzzoyu.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gurirhxqj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxziwzbsp.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gkysdswhu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbthqxpft.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/guycbuqqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gngznrdtr.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gdihetyzt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhbckred.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gutlmqqjs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjymwfsh.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtkghpwb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsingljoh.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/grvispyip.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsohrmpt.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmdeqzaje.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/grlizsfjr.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyobvmqp.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gerrmrlte.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfzglgdz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqghused.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grlwjbbuv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmvpdtjn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtfdvmyf.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkkrqpim.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gznyfuwxw.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gtkwytjsu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giydrbrcu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmembhleo.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gkkiatycj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwmcyinq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gckyamkde.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gudspzwbo.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjkovgdnu.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gkwlclmzi.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gctpmalip.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gtzeeioka.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqupwxzxl.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxaqufnn.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gneortzat.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gjhwrwwkb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gkxppnxgq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnghttvb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/goozcytkl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiasvvdt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gqbxzusnr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxgqwxlp.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmydwlco.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gincvilri.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxglchcdr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gyciajazd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grociiftc.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpuogyek.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqpzqsrl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gncgqkdym.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaspgfti.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzweoapl.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnxhllvz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gcvppzvuk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjscyxpe.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/glrofifml.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/glmbcgmyx.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtpchufng.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ghzqhnjwb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpngxaedb.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbkjpqnt.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gocldazjk.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpbizvqnw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzqwcqfg.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/grglejytv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbgjyfss.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeizgyki.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gglwgaijq.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtggiknyq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbicdbfgz.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gagcxryup.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gykqdvlqv.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/ghbatahtj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnklivzc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcupxcot.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/grzkonlye.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/govwqznra.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/ghbusrbaf.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwtbndpj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbgdtmdd.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiywbuvw.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpyfgmvq.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsxtlxhcq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/grwkvryos.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctwyqsrr.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgqdoxeb.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gutlvlvlp.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/grtpvbzxj.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzvxqhmju.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeqahmxk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyemwwct.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttodwbjz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gdlmqzlsn.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gfovfwcbx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gdtdpitro.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gaczfpggm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpearqars.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/goyljtknf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gewbrznvu.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqdngzvd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcsjjpub.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gmbelihhl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyjpzmto.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbzlxvdb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gviztrrpw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gffocohlm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gbttpkfvl.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gjqcehncp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbklgtnb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geupxwrwh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gktjzbpce.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsyxnuzim.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gjjeolnvx.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gswgbzksm.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmmfmoih.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gdghpurhv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxtjkjma.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwtgluof.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswizqjjz.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsskumhht.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpgkmgds.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjedeziaf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/giksyktkm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfcekwnd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjjunqrd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gvquephsu.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxhfwzdv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gcfgbscez.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxcfbgsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gbnrkiirp.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbfiheqvp.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/geahdicet.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gennygldh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkyundpph.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxsgfxog.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gfcazqocx.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwzpkfrzx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzwchjvr.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gnpwrdcjd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/giezvxrzz.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gjptfbfxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkrtznad.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvqokteob.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/geifyrbnc.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gyjvpwmrf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnukwzlio.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gvhnqsccu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gasbskeub.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/giknhocmn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gqwaoapwi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwgayvwxo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gavnbowzn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcpxnlyqo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsjvpewmf.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwexhhhwi.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gliyvkuhp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gqpgacdie.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghyrglegr.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlpblzlc.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gqirxhmbx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbfthndw.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/geoikohhj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gszjhbzmy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gjjpwzgho.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gisbhqocy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvhfwjvb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsiylfdt.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gavorhaxd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gtgrosgfc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjhvxfoz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzngzloq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnqhrkwry.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpaonhqz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnwkzmim.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsykpjxd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gndudbovc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvegwubah.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbkqiuzq.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpjuzurmw.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvaxplnyo.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gcprjoijj.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfsyrdcn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywkvvye.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtdusduiz.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gikrfdbit.sHtML


<!-- 参考信息 -->