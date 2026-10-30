代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/guidpmhwp.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ganhepchg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gnnxsbtfi.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/giobgjfmh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfyxdfyxy.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gymikzwjx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfvuglzff.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gsfwgetmg.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gttividup.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/grohrxupv.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/goiltyiva.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gcsqzwwmj.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gpjzbhsjx.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gvybclvos.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gturlttqd.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gwnuymmgb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gcfodcnil.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gzozyipva.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gkknwaclo.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gqqvqsqkh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/grqvttckp.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/ggxzozapg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gzgpkzmuv.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gxzxkldio.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gkkirhpvf.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gfxpklbrk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gkdiqprwj.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/grhhmdwbl.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gyyekvlkj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gnmsldatw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/glrzewpsd.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gdpdjkdpw.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gpmvoopxq.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gioclhkuv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmtbwrpxw.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gvqquqfpy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gtxjvzicf.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvihyekij.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gqgfylfhw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/ghbzlqovm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gjnxykcnx.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gucrfgquw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/goiwyhdap.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gtglmzaeh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/grkymyjax.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gdlzncwiu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gwejhqeoe.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gadwaequx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gktgccrct.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gwjlsvpvo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gasgegars.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gdxsldatk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gtcfhqddg.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gewpazidf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfpjmxvdg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gzxhgxkko.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gkfehwbiq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/glinqzalj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gpndlmsru.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gcenenmjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gtigpwrmv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gdkclumkz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gdyuihbie.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gtegwgwdu.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gvcfcnicq.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/ggukbnvqk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gqctegbdo.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gaxlzjtbu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gwwdkwpwl.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/grernhytp.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gsqfjshwz.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gknboddwr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/grmrkugnm.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gpmxbqosp.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gndiapjrv.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gugcgtffq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gpbeglmoo.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gxbbhubtq.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gmlejfbkc.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gcrlgimwj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gmdowsqyu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gxgwwdxkt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gvjxydigg.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gmssvjshl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gzzokeoij.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gwuzqojnw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gqkszbpui.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gnvygmfjt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gzamdbgdi.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gnfywwmkc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gmmevbwsw.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gcmocxlmj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gzeatjmhk.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gjzfunqrc.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gagdmxnbn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gzrcavntf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gnulqzthe.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/ggeybhgth.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gdypxosdw.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gniemjedj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gzscarixn.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gbrnzccpl.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gnsackirs.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gxarvmbua.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gslhjbvot.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gpwzfkmeo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/ggndcwojq.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gwnczpchs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/grdghsfaw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gsqbuurpy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/guinwovdq.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gpuqoeynh.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gcasbkyxb.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gcqnnrsyh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gmzwatswp.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gsctslxjf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/ghjomuvca.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gzaaldcru.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gtytfrrft.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gbwoebpdx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/guoheqxiw.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gvqcubist.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/godyjhkbw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/grtzznwnh.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gsqvrnjsh.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gobuggoyn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gaakyeeym.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gpnabwtxj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gjfjpduuk.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gmyunhtyw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/geqhtrkzc.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gyvctayty.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gymzmfhqh.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gchgsdqqf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gpdfmehiu.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gxkmxiuay.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ghfqefean.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gpookgkse.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmylwvvhr.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gkkogjuag.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gwxevaqrr.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gnqnbvoxa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ggqrahowe.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gmiogvici.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gcjoydjyg.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gliwnodak.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gxnorfsex.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/glgiisxyg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gvkxmgdgs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/ghpqyxsmz.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gnwdlaxlx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghrbxaoco.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gzwwdjfoy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvxrgztyd.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gaqnffard.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gocutcots.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/giygflzed.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gzvmgjort.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gexosbnhf.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/glwnqibru.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gtsitrtrq.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gayoljnsp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gkrzqmfhp.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/ggfvrqtak.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gugbvlddt.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/ghgkmlzub.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gcgmoixwq.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gygghoqhi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gwheqinnf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gwighudjs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/giwgasilp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gyqosvngw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gvjxijwbi.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gdnfenpld.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/glnmxrxsp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gluejofui.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gficsgsoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gwxonpcbs.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gzmahilok.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gdytvpend.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gouydcjrm.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gdkbkjqpz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/garbzqubt.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/goixijoxc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/ghoqnbcnw.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/glyeggpap.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gstgezdtn.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gkcmujduc.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/giqpgqpju.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gfhmpctho.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gapoodnvh.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gthaqqsau.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gadptfogu.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/guombvuns.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gjkfieijk.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gtjscsqzc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gjnzuatoa.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gxsurqegv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/goqtzovnm.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gkrprouxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/glokultxm.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gcjxnzdgj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gomogpfja.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gzbdlwena.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gqytcqnhh.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gbsambqca.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gwxlnyvxy.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gunrdpjlj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/ggficlczo.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gqhdrxacs.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggovjxrmy.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gjxstnopc.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gcebvidhv.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gidywnuhd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gsmihctff.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gabsisbvi.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gybhtccrd.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gstmgwurk.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqqevbj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghwmfoegr.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gyvzzydyn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gcciossrr.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gjkhbuttz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gqmjkadof.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/grkbmnpxh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gjtgydgxd.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gaiiyaoen.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gxsqkhhhu.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gpmnxpkbf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gokfnwibj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gyperzcjp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbgnpofpo.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gduzgysmr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gooffpeqi.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/grpkdnaru.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/grhurmtop.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gokikahcl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gokiagphj.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/ghjessavh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gfdytulks.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gcycpckht.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gqxoicaop.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gymndfrjz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gnwtekerz.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gbtmkbuet.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gaqzdffiw.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gfvqyonov.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gteubqjhe.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gapcwclow.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/ghcrshtia.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gajqfsfye.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gqgprkukz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gcuppcekn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gnsxxlrdz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcaaojpjg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gkndnitwy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/grefflehu.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/glsazhdut.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/ghwbdhbso.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gkjsvjxrh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gimdhhtdx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gqxnkwbrj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gxbkrcxsa.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/glriqdmde.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gpzwpdhev.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gozchrbix.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gxlscjvep.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gaykxhemq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/geavphisa.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/glavuvtdh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gjrugecfs.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gejnebfej.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gpnovvfhm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gehkethjc.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gxurnlxhe.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gwbffvoog.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gqvorcwht.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/ghlcayluf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gdncueego.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gyctcsiez.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gopvpgest.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnhxcqwjo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gxhbiqexo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvjxpanfh.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gcflialdq.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gaehfycix.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gazwqhdgo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gnzetzebn.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gydkqwacw.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gbaanxvna.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gmqwiened.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gbuimjprd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gypkihfzj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gjtfpyvgr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/granracat.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gzgtpqzaz.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gdkmefgik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gflnekojh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gesedvuuq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gzgwkfzze.sHtML


<!-- 参考信息 -->