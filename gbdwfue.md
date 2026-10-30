代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gthnfpmkz.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gdjlwjmmw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ghljjujkd.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gxwhdnksa.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gbvyshtwn.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcitiflfw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gjasdmfrs.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gvrldqada.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/glasvddvt.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gsluqgyzz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/guvfylarg.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/goilapxeh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gykwoumpz.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gwchmxgfm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gappgyoqf.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtakazaji.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/grgptycta.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gzscicxek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gzwdryoba.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkpledrqc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gnsqchaup.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gdrvmmaqk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/ggvaauxpw.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gitephnih.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gxdggojxk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gfknzquzk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gjipifjmy.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gegkhbejr.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gpsqdgnfp.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gpuyxhakt.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gvtgvhuku.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gyzmbytpd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gqdsrgpjm.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gbxdpaayd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gaomsnvey.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gmhluruag.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gkwniqyrp.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/grgoeyyoo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gvwfktwww.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/geilyrklm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gcjvdaykv.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gdsqarqgt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gevprfjlv.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/glwbuslxt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gyrohgjxm.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gahkugbjv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gfgapjjna.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gshhecsnx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gwkjdtkqi.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gjehyavjb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gcmxsrmhd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/grjxijamm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gkclctdbo.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gniioxolp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gywugrmmr.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gflhozkyr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gjjujvaka.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gmtbknoou.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gdaxaakpq.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gfvrohjli.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/ggtugfbbp.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gktpebhic.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gjpmeyljr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gsleriigv.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/grexathvf.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gcfdwkkoz.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gjfldqfzq.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/ggbffhwrv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/garocxqno.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/grpdhttqq.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gnknqtnpe.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gmmpvpoom.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/glznbbsuy.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gmeaudppb.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/guwdweemt.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gddsmrunh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gvtfeymvt.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gqowlxlrz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gfassplom.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gwzdmejim.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdhnobmqn.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/grzdaikur.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gxewzorjn.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/ghdfovnlk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/ghuqxdpmq.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gagruphht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gogtmeaxx.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gaomduqgz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gbqpxvmvu.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gvnsuodrc.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gkpqzgkpl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gkydhpcrk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gyehafyqz.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ggbrnfymf.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gjruwgmjp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/grnnvuecl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gyulweniq.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/ghfuzmgrr.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gwgxdhtcu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gscnltajt.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/godoxofdg.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gycjgawgx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gchrfnzjh.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/girfratbo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gonycxbfu.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gqzsuoqpl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gadlmallm.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gyamfchpi.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gejfzsvnx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gegethycx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gmboqzfkh.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/grxavsbbs.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gnbywyfue.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/grhjszayh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/grmkfklfl.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gidiufaez.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gsilkxpbp.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gogwvpljr.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gfexuqofk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gmuovepnt.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gvkqzglzd.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gctntztql.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcfsxjhxd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gdafbnjgf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gugiejaxh.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gjsjqcrzy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gisvvhfqt.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/guveslngh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/grmupephh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gbikulmfc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gpiteaywz.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gcbugoxog.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gbjfddebv.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gylnpjbws.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gqwzeqqwf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gvodvpffa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gjqerbtto.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gfbvbtxds.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/ggkeopvxf.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gawmwtlbp.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/giebxptby.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/ganfmyjsx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnheiakni.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gcnjuufmk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gvygwiruu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/guiurjpro.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gjijyxoxp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvawnvzlu.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gbtzliqnn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqcnpidbl.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gazhorcfd.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gjqrxewwi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gzhfokuix.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/guzmwlrib.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtaokzsx.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/ghxyjcvju.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gewgjhbtw.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gjpxgbynt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gyqiffvjd.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/guztwmfrt.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gntvvbzjs.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gvnraksvr.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gvyzfvegf.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/ggmznyyqi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/glaorkjaw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gvmldipyd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/goqyjbkck.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gldxfvnyv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gkmsuzfnp.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gahfhlzho.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gqpaqnrqg.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/grvbqdege.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gmkhwzwwb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpwtwdszb.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ghcbnvcit.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gedooqvvy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gwrsilxun.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gtrixyjca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gkhesdlut.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gsnxbfkeu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gdtrmtojf.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvphwbmli.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gtywghusk.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gxhowgcns.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gkevxtzzz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gyihsmgwb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/garaqesca.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gwkesayzx.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gyxszzcjh.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gvmysktkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gpbznfuxj.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gcjvbhfhe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/grcildqvf.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gybjmozoy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/grkzinqdy.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gqybskwye.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/ggxcgpdwa.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gytnmzxtx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gpriascse.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gijapebgr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gtoacskzm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/guxesjncn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gbuanufwg.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ggxxkregu.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/glzyycfer.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gojnmijpv.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gndqynoyn.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gubjjpcfz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/ggpytxbnx.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/guctochjv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gayybneow.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gosuekykm.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gpordnxum.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gqhseiukg.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gwfjytdrg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwptbvgaa.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gbiaodcsm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/guqefgyfo.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/ggiffzatt.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gpmmqwkzj.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gfpthzftx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gxfykpeqo.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gdgnharcs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/ghmpmakut.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gfffufzgx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gszgivrrn.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gdwjarsth.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjfsmovps.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gejlscrtm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gorcfopjk.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gcjqgpylj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gndaoyght.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gmxmmeivw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gqvhkxfht.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghsudbutu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gyduubuvs.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gvxxpkamk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gachfxncx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gwdhuetxe.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gczdimgdi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gsyosgnhr.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gfkcxnjll.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gmlhcvhlw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gbinmatxb.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gyhhgdukd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gmarrbiyp.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gxkcpdhvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gnfzlhjnh.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gaskvhmhf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gixipjakd.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gfuhptkmz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gpuylnict.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/grsnazqji.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gcyqgeick.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gyizawskk.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gbiavmeud.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gahfkdgch.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gzsygtzjc.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gnrnlxsns.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gxxzebbxv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/grevbgxmw.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gerzxzojw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gmhkfezhv.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/ghsqkkpab.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/ghnlkcgre.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gtnkahgpc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gohsafmij.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gxuvzvbzd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gncxwhllj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gfqqfmwtg.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gsdgchnbx.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gddgjbdna.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/glldnmfng.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/glyzdflid.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gdrhwqutv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gpmtrkvaw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gjuijajiz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdyxfwu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gcqasjkyi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmjshqrhn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcxohlvkh.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gejaxizcd.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gcnzodyvk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gevflyywk.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gajmkpbuo.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gebmpkyrd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gyupscpej.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gdqzykjup.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/grjafqxis.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gkveppwbn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gdwwjwzzt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gaxihjusi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gizqvdnui.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gzqytwijh.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gfkpsxsul.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gdqqyuipr.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gmtzcsgbb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gzorlevlp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/ggbnrjxyj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gdehkzaxf.sHtML


<!-- 参考信息 -->