代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/guitjbjli.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmapxbgjd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggavtnpjy.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvxesoff.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaagyikr.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcqoqolh.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gujgnuzvb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdyampsw.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gfurefbhv.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbceyzxh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpzpldqoz.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdhaybvx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpeqfrne.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gmpazhmyt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkvfdjqx.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbvmsdjsy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gonkvcttt.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlmyvqdi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhiltxod.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrgjqfjd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjhzlxre.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gwgsftccn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpbijiwv.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcxtjpyg.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giegjoomf.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gabwgvakk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaqmkxxw.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/guksecwgs.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsuwdfib.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggetuwdjz.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtshinz.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvgpahvbg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbjpwgkm.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmkjkhjdv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrzrintn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gevsgldel.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxnrrjwv.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabxjbyko.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaasxang.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunogngzk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gjgkkphoz.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwkplfgl.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gcmefnpak.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjvlmtzf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gtwwjevui.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/giinhgtue.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gstgsmcar.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gopcvrpyi.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmvhqsvyj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonfjljrp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaxfbhip.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqxqnppxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnafxbbd.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gcgagpezj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gserfhbgq.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/glpfgkhla.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galpuqblb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gxbvuanse.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gowedlrkj.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gniannxkb.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzlbazjo.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqkkncd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkqeitvp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gezkekeaq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgqsuzef.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikveifep.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhrcntaa.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfklsjxc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtxrvvsy.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gtqfjyvbo.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvittnpz.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxfiwafgo.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gbebbzhpb.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/ghksqekwd.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gdmnekqog.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gfosvfdqf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/giaiybibb.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gkfbxfrdc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/glemramud.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyllwntnu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpzdfmjd.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/ghfhcuwny.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxzmkqfc.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvankitb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhdnhtxr.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyhmllfb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gihcbgwxu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiqkyfcu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gclblsfti.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/guhbbcuxr.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvofnttjp.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gpggfwmfw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmwwfdjk.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvruoynow.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvixkadfc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwwsctw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpweuwly.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjupibzw.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvwepfbf.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnzmcbrx.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyimfnspo.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboclybot.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzbmyhbf.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gollamytl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gohnqotae.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrjsrnya.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gnltgjfcj.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/grwmpzywj.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/guqqlkazr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyatxpzuq.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gyxetuuqb.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlhbosre.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gqownjilb.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjpnnwzk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gchfwcnlp.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gkpekuwju.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmtcopxw.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/grujcwtip.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxakjclg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxpjccwc.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gupkxrefx.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gcbfddqjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glnucvnkn.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeveofdq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gfqdjwhkx.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmdrhyefy.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gyolhmypb.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gchnsivyt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gabwvecun.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/glemwywzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggpgmtoxe.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvxvpkiuw.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ghzbnwltl.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdmaaixv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzanveaq.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfvyvemkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpskcfpq.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gksgfhflr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzzcwbqw.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/ggulnjuhv.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gcvycfrzh.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgocgxvo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghfgthtkn.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gihiylytb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrflzbcp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxfatxyi.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gshbhjqjl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbmavqzb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvkicrdb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gclxwgbpy.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevbkhrql.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwrsejax.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyidushuu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhirduzx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/glpcrilen.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoywawyr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/galqlwtbd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gmdukrjhg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gctuptlkw.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxwbwgbc.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxyvgjqsd.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/guntcrhoh.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gioxybfvc.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtneuoial.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjfofcyk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrbcpkeq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwbdfzer.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqmeepuv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ghkiznici.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilatmjeh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gcmdswawf.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gduboqjjw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmckqzli.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggilludyq.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtavgxjw.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmgfsgzzg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glodxookw.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gezwgqybf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgfscntd.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozrfgxff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcopongzu.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gadqxrrgj.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gifhuexml.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gpaaumljk.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasxmdgas.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbzrjougu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gskaaccom.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjclnxbd.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gykjoxjen.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gryidciot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gigskidgv.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ggrbzyvpy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gifiwagbg.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/geihloeyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsrccfed.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gajrtxszq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gtmzjifor.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gldvutqsn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gnistesfx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwbxnkly.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfkrztmc.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gccewwnyo.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtmhlbjz.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gkulhgezn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmeqgbbt.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjfuhusj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacwcrmsa.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gukfwtuxr.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsolamonq.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/grwiqtvoz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklujmtac.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvosbpfu.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gfgxetdko.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpxbyzkc.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gqojpumii.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwdsdfthi.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gjxytsctk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goydjdhqx.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrpsmjpp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdcavxjo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbilpddh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gnrvazijt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gmisuhxis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuvjezuv.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdssexzv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhcdxwvl.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/geldyigpf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzwonxkoc.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gohiurvss.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxpucwdq.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gecqnslov.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjpbzuxr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrflzlm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gottnumkv.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsohkxste.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeamqntm.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/giowjtbrl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzasbakh.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvqiskpyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gagnicqmm.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gohjhahrj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxpfcyfc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzisrvmcw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/guqljnarc.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoqkeufh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gezczxzek.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqoihfey.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmydqomsy.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gogertzri.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjiesearb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfmixnux.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gwyhjsbwq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtuiawzk.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczbxfdfm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gphozrsob.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gitcdpdqy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gnwalafyr.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkisqhuxx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfcwzoww.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gaacwpydw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxfwjtxvu.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gekdeelet.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/guvvyihmb.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gduefnynw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/geypgkgqb.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gnbluctgm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/geqovyblp.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzqovtmu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbmzduys.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlphefbe.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocuuehlg.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbcjgfkf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqamrltga.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gydrqjtlc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcyrkneg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfiivfdzz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/grohwebkd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gccgnabpn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gegoprkwo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guuzriydp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpobicyko.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbtjdqvad.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrjszfio.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gczyhyjfm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxopgqxp.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gclbocpmg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqifqvsk.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/ghkczuvvb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gsppwlylz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/ggbwwqmkd.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlvpjsjt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkaziliz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggrjegwmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gduzrltnw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ghivnovym.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnizvrqe.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guopruxmv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/ggkqwshff.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gnqtmmbgc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzdcpga.sHtML


<!-- 参考信息 -->