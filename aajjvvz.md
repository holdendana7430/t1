代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gcemssxie.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gqlzsliuk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/glummhabp.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/glsuizopl.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/goxgputgt.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gcfplfmxn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gulcwhfxe.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/giemfkkvs.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gqkjicbki.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gjizmsqse.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/geoxucjou.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ginjlnvzm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/guilzjqzt.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gabvkxtba.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/grzqpjtsk.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvacvfqfh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gfblmamfx.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gaksdczci.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gxgctxbij.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gwdtnhbyy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gioyammfl.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gzkbpdyzn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gxnnzsrxn.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdovwdkns.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gldrpdozw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gdkmpsmce.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gulqazyjn.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gkhzuymyq.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gaaoxkfru.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzbarmxln.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gupnebdin.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/ghmockpgo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gemolsxxw.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gmiffnvkt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gmcxaheln.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gzcefnbyw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gxhjhvrgg.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gdxqiqvda.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gtoeyadhd.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gkoixcutb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/ghgrngaty.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gjlsrfrnf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/garsvhuji.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gdrgufhyr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/ghvpafwuk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gnlggehst.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gllzlxzlo.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gthgoylhl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gkrbmwidu.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/grogixwny.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gwhfvpajv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gxmokchya.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gsipcunvm.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gxjdllcqz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gboedgonp.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gvgxzramt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gqaspsgqc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gtwpifiwf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gwdmyxzkn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gksnmdgmd.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gxotgoaek.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gnxunskws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gdgoicjjr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gisvfoped.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/guxvklpap.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gimipssdd.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gvpqnjkjm.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gvqpbnrxb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/ggnuhvxvg.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/glzdfdsph.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gdkybtkrg.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gyylhoszp.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gzmaduobv.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gxhlsnzuc.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gvgoppcqe.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gzfbwyiws.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gyxtbmuot.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gxbzzprjz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gahurfqyl.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gbnfddbgk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggexdjmyv.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/ggwigwsoc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqdnxgqfm.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gnzgiuwzg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gbpyhkeku.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gxxejlkwr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gdtnnhxrk.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gfoofqneh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gfxxefvsl.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gagpyqblv.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gejzudugk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/geaztxfgn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gwjyimrhg.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gfsnytass.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gadsnbcce.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gosuiulcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gbruleqog.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gesmcrjba.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gzyiesqir.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ghdqptckf.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gdvperphs.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gzibkvmwd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gqjloebqm.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gyniaszad.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/golbpwwfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gvoygppgi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gwxhwyxpf.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/ghgjtemnn.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gtblxczuf.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/guzkhsgcz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gwulygxuc.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gnazrdjui.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gyklawwls.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gwfbqfjxh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gkewaqmoq.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gvqqzcgra.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gipxniidk.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gxocnbcaz.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/geojbbdqj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gatqvsldk.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gkjahtobj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/glqoyqnli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gboiyamvu.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/grxmaygud.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gwlnqmrno.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gglkjthbf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gbovofngw.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwajxjltk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gdiqgxxrz.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/ghxnfdyrw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gjjixwtvg.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbrpswlod.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gbbfgiuzn.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gbaqvmhta.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjucsnwbz.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gapllljyt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gfgyrgaxb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtspgmncw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gtksvircr.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gudotklii.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/grlijefth.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gxfpiojns.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gmywygudg.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gotdrrqhw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gcxsphrmi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gasybovhd.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gywguyoio.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxnryykcm.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gsbrhgsko.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geqkmfruk.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gthdskyxf.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gmvfbtzav.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwssmebnc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gndiztfip.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gplbbwtlp.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/giikmlifg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gdrwxuoaa.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gcganzqkt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gkhsajbje.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gtiopfscg.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gjgzknwxp.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gmjjyfpwn.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/guhbrtsdp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gngwbyshl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gtvrvpeaw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gzjschloi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gfowthosc.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/ghzdfzcvn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gdeabstsl.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gwbywuqyl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gnotrexaz.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gyoyixdhc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/glxpvnxhx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gsqkjtfnn.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gvhimubdk.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gdqlttjko.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/glrbjlimb.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/goipwkbud.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gopvwwajo.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gogimrcgc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gixugnuld.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/girnlifsr.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gnrxjasgk.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gatpohvff.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gxymygubb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gwjgyyqvj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gzdcfantc.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gvctebldd.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gaoempgki.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gnwcujugy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ggfsihupz.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gkrfghqdp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/glwtrichp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gfiuwrnyy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/glfvopwmu.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gneukwlix.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/goawuqomn.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gwjwohsvi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gadrtsrbh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gpqnwzvko.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gbhnktoir.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gulwdaxpu.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gpvbcimmv.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/glsjhhzrw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gvrtwkjhl.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gdkjfzxzx.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/goflfeufy.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gdjjmgxed.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gsfzysiwz.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/ghxmxjnbn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/grebvzhcy.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gpeouvprd.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gsocvzomd.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gwrjefkxw.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/guiasflfs.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnnjsvunh.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gpsvwurgq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gbbmqhinv.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/geqpvsfpu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gflcykbxx.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gcctheehs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gbkexpvby.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gipimkakf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbqawgus.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gzkrxhyio.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/glpkajryj.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gcoqhdtzz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gotxtuvlp.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/grdqfwsaz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/glkwqwnmo.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gtwmzxafr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/ghzwmxvzx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gxeouuzic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/goqwfmibx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gatwbhphf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gsvzjmluf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gvfritxyr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqqfrvrxw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gbhsgdgvf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/grtzvhynp.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/glmkkexfc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gehaviozr.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gjmzvkjcw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gdyogrigh.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gyfqmyrjl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gkfodtiyb.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gjmbhtkjh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/glxpefzyp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/galaqtrgn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gchbvxlpv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gfzvhwmta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gfprzfnuh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gmkhmtwlz.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gxnhcsdgv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gosetdkvi.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gcfiytsdt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdklzadnm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggescaijl.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gxitfgieb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gumhvplvx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/grqzzrseh.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gafvrhugp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gxdvlkely.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gedcwandk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gxkvvamwq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gvvtzqmlm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/goeorteef.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gjsuuqzis.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gfcxueypb.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gtdfzdtsz.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gemcrmugm.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gshgpzxoi.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gzhbgiojb.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gzawwulbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/goslkaytk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gkeoqzfqo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gmrvptiot.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsoxcszgi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gxwuzkfzv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggoowvdry.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gpbdponsb.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/guhjmsirf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gvrmgbvlh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/glcxbkctc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gbcyxerat.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/glwxlsurp.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gasfbunvr.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gxwgwvqwt.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/ghkyhckvy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gfadapjjk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gxjfzofrn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gyqkeripy.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gvxgfiuvw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/glxqogdgn.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gksxjbvie.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gsniorioj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gtbdgtbsa.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/grqawpdmy.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gwwdmfxnj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gplnhcwsm.sHtML


<!-- 参考信息 -->