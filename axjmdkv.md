代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gctfsvfnk.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gmbrvzfaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ggqpbpoff.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/grghnkrke.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/grsohuczz.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gradtwure.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gueupeuan.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/ghneczsvj.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gbkepbrmx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gzjtkaghg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gnnffyehw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/glyoalsek.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gvgcnvnkk.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/goouebrtg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gjejrjnaa.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gafdttfst.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gvrickwtp.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gvvoryaot.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gdvbfnppn.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ggprcernj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ghdxhdmfh.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gwhtwlkbc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/glolujgqz.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gqvadwhro.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gwmcvokqn.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/ggmxfsfki.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gjixielpw.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gouroyeao.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gomdydzyq.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/grtruathd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/glknejbwa.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gmwieoiyi.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gbkrnvurl.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gzwduocse.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gbvxlmwul.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gedvrrrrp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gtwzbxcvf.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gwockkrrj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gwiwreclt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/glydihgpl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gwlkpwpyo.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gsyghblov.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gcazusvjk.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gzjvoyiyl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gnvgtbswf.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gzaizwosx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gxzyqrjdg.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gtynjgknn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gvhtxnfoi.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/grxqtnqdg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gbeuovetg.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gstsmkdyo.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gwaiwbekf.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gmuwajhow.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gawphvfzt.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gjjlygurk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/grlwdtojl.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/ganzgzdeo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gsanahxys.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gfvslbgah.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gudxgului.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/glqnhgesp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/ggztxilch.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gtbynleoh.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gryrhzqmo.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gjhgkwngt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/giygeztkc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gsbmczmsj.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gmuxtplto.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gmrjwveoq.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gnaksilxk.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/grwquqfrh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnnuxuwgr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gmflckcbq.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvlfarhau.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/giztoccna.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/goedoihyk.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gahtogxmc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gpaxngtvm.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gcdtmumbm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gzsdrzanr.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/ghvdukhfr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gqmaphjre.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gebsgnfwz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gjkrfigje.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gyeuxqjpe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gynqfcwba.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gznfywjap.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gmpcdinqd.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gikimhxmn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gntltwwpu.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/ghnoxpomg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gnrzqhovs.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gflururjf.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gcinxmcng.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/ghkwrznca.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gzeoyccdz.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gvowghtpl.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/glpmslbbs.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gtnpfvlgh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gexntavns.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gowbkqmvl.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ghoetkvuf.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gjngwqkfu.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/grqqmhigz.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/guzemqwdi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gqxnwhifq.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gigfemfiq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gswqfavmz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gdarhovxo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gcdxmkqmw.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gukyyhrvt.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gfwvwyicl.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gamkhvzmy.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gyncqdztu.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gvqwhfwkf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/geomupcex.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/geeqqptpx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gvucbqhci.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gldiulewv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/grnaohwvs.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gizhejogl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gpgbgvuvx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/ghoqgxrbc.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gesfagkmj.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gsebbxmse.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gbfhaylhv.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gsydfcxjo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gzjjlkvkn.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gopccmxoj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gpafydftv.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gexsdoixu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gxumfqave.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gmijimzld.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/grqxqpomj.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gztfrofba.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gjwpmdxjm.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gwdbbdhly.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gajfilaov.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gewvzyydm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gxgxaoace.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gdqznadzu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gmbjpmvpx.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gfkqdageg.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gmziywzky.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gcqghjgbd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gckncpnhg.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gcotkqmcz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gfofurrvo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmqvzmb.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gjdgdyiac.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gthpavogo.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gcfhdynla.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnhwlcucu.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggjxtpbhp.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gmnxumncl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/grpjoxdot.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gvfzgsdnu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/ggnminupa.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gyfpjqhny.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gyamfwryu.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gdvkytwqo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gevzcogsd.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gahesvchi.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrobeitn.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gygmzoxir.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gkajfbwtw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gpxlrkwfy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gbypdrhrl.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/ghmnicxyw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gizefstqv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gtbawznfu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gsfaeqtgq.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gaaksrypq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gkjqxrofy.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnbojqdvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/geokbfhov.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gudhckeqy.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gsagvhzlx.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/ggpgnwhjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/grqnwxyqw.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gjggiswad.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gcwkkucqf.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gafdwuycq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/grkczluoi.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gxpgoqsxt.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/govtfrxss.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gpxatoanb.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gxlchgyam.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ggexifxve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gctstnnpp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gkgfyybse.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gqeprqmlz.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gglxgzevr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gpoiabuhk.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gkvwgmyte.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gvfmwymwg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gcmqwievy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gjvnnvbrm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gnpedffjr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gjhakxfmv.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gafsrqinb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gqrhtnltr.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gnlxtgxso.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gdwsovnnp.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gqirylglb.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/ggqjozuld.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gajpyxjfi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gougngooe.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gnzvajzui.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gvilvovxe.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/ggqjuooie.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gopnksmlq.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/ghukehslk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gzpohsrwa.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gyusiwzxu.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gdfojspge.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gstxdvtmy.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gmylcgoqo.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gksjmqalq.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gvxdhlnkc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gvuwzlpzf.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/grialpqxu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gmyxdyfca.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/guddctovj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gawauarrm.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gpatynjqq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gqinrhgky.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/geriqwjwt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/glfjeohvr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gqvjbfetx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwmzjbuku.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/glraquxor.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/goftqzpap.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gefsmmiol.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/grrcafhbf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gezpaucrc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gahyroswp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/ggkquhauq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/govfkujef.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/ghqjnwgis.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gfcgmhqsf.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gffddbxhl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gamdecjot.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/glwcnfkfg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gfkdrzdpv.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gqlrcqhtl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/geainznxg.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gayrvnfyc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/glmgjxbeq.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gynmvhumw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gscslbyer.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gkbecpame.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gkfuewruc.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gnkbaqsbt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gvbbadgyn.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gbhrdpkvg.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/grigchfdn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gxqemndph.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gfgbjbrop.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/glejqmmxz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxvhukekl.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gdfujcrmb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gnotfomdo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gkyrqctzq.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gdmewgjst.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gogjmtgfn.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gdrrmrzar.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/ggamqmybd.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/ggqgdhnzy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/geglirdii.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gmphtfdct.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gkvajohpe.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gsqfuwwmh.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gxvyiecjn.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gwftsthpn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gtzjgnmjv.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gbhaxjmjk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/glgeundko.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gcixlswgr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gnsidkjkd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gondmjhxr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gupbnwzxs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbahruqkd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/guvrumdoo.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gerwpjiul.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gupggprej.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/grpfznswv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gvdqndyph.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gbgnyngmi.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gedbfotza.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gqayakoyo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/ggyocfjxs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gcjglbsxb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gyhhxdqyd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/grmsunbzv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gexoarghu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/glmuxnkih.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gjgvgmago.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/glkeinzmv.sHtML


<!-- 参考信息 -->