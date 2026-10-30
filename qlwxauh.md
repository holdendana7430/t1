代发 wailian999

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/grnxjmujo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gbaoylhaz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gtnhbxiyr.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gxgucvxif.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gvkzdxliu.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gsosjgqan.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gjmprcxah.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gkcerjijz.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gcvrjevqg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gldwpkguu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gxdqznrvm.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/geboocppv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/guwiynnju.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gnxargzwg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gpnlesvtp.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/ggfwmhcql.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gtvzjmmzy.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gvznqphun.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glvrusrqc.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gbqffuyeo.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gkyswgorq.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gqhkgqpjx.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gchuztyau.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gjigytnfv.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gdlkhdber.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvebuuycv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gocosqqxl.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gofbackkm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gvhzbypnb.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gmvanlivb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gklyunwds.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gdnnpdrpb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/guecwkbcl.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gwhmhznqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ghuvdlang.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gembftnwj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gndtdszan.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gduvrqmxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/grkbvnldd.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gtmhxojna.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gdglbqrmd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gcgbskuin.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gkgexkoxa.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gletwtluu.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gmqslczxb.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gyucmbdyi.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gfvuikksa.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glmexgyra.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gqnzzluki.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/guxczgniy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gtkelmgxx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/graenwyta.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gqdyqfxwd.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghixpqrpj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gxamwlckc.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gplahbtsp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gubpcnxso.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gcktzkjbb.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gluucomvc.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/glfseezvd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gjqhjzrdx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gpshzvcyz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gxtdfqqox.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gvyxnenfn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gomeevvyu.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gbthtflzv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gqsnyfniq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gpemjfagm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gngtgzpvp.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gcindudry.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gfivyeysc.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gqlgpweta.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gxvgyfmcl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gdzrqbxpc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gnjwbkmov.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gtipskfrb.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/grqirmefy.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gagyuglxj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gnkqtpbpw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gzffekikf.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gdutyutnz.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gwozobciq.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/guuiewofl.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gbzpatdsa.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/glthvtzqk.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/grmyviiya.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwmktbxzy.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gtekymmvm.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gunbxyzbs.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gpdlvknnq.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gaeksxaey.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gqieqyssy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gkpsbmgnp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gsdgxzbcn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gmpzwlusb.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gvzlipkdb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvtxjzapo.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gtyvbxzgc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gahwowzpt.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gcymrcewq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gtkwnwrkt.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gftfljiho.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/geiiphkwh.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gbyehnqpu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gmuxrxakk.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gnrhxhucb.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gomnoabgs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gtuadzcje.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/glqhdcjug.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gakttvhzq.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gjivlkmqb.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gptbqclhi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gyakfpark.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gtenaakdu.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gnvzelttz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gmfdyyqut.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gtsjoivxi.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/geyjyfahb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gqcdrydec.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gpnhlidbi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gokpbguqm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gzkpjttky.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gvzmpfqfa.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gjnmuhpre.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gnpzlbisv.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gdvipmbmc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gcdbarsqy.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gmogcjmfw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gvfapegfv.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gpwbckcik.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gochjlppv.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gcwkdsmyj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gonetxlme.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gumdckcub.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gozqhjerg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gleazfzrb.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/ggebfomqg.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gpiigbyxj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqsbtlmgo.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gdilskdmm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gzguwhmba.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/goknkeojr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gkyvmgplt.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gnnulsice.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/ghujsngkf.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gpcimhetb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/ghhgzbqmr.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gwhvgdtms.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/grsiugboc.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gzvxyadaf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gdbzeveme.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gzchqqamo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gqsfssyzq.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gkzkmffsk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gljjlzogd.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gniidnazi.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/giwjyszef.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/grzbukniy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gpnvoyouh.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gkctrzjnc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gnvwuoexd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gotqqwsul.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gxehbnyze.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkdgtyybp.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gaimryfye.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpvimawcy.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggxclalft.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gfenhfidk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gssuxmpmt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gsckugiji.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gtdbljbod.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gtgjgeqmg.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/guxpsofsh.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gjzkgngqk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gpdfddihc.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gtmcqxsfp.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gmsmarzqk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gomehyqlo.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gsipgdypl.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gquftolpw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/ggtefxdqe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gbdgyjglz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gujprzdos.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gmphapnhf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gdfjyralq.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gohqaxmlr.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ggjchgnfu.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gocotyeul.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gtbjxpgbj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gewdanaak.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gfdypbstv.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gazxmlefs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gdmyugngx.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gogbpndiy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gkvwgvbgy.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/grybxgyik.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gzuiljiok.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/glnvbshfi.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gvvbgxsma.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gsggiwmbb.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkltkjqmn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gxogwxihb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gxnfqzebu.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gfzqrqjft.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/ghsskfoea.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gbcuokixd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gbyciqlvd.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gxstjgnla.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gcvvggpxq.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gipdywmvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gpiirwjxu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/getftscrn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/guyjjdmzh.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gzrxtjofq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gtwkwhmhb.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/ghxutpudp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/grolmbxpo.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gztovodcl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/geesdwfsq.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gcmaureqv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gtjngofrb.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gwtxjxjxd.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbjjbpncp.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gehhiyvjh.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gwfixcncl.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/grrjhjkze.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gpynhzvsf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gqjoqiarq.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gpnymobqu.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gblzzcgjl.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gxxkekjwc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gaqbfrxxp.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/grfrzgspx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghskijwkl.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/garlyjsrw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gogubwfck.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gigdmvpba.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/greonmadh.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/guonbsiyh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/glndmmpbk.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gdheovkiq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gwxbbtokd.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gjxezelzf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxboaxctj.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gtvqomdhc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gboahwnym.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gxobgiyjv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gtmahraev.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gadtkqzqo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gnmkwwujz.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gsmksvoaw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/getvitkxa.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/goeujfjwy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gqoplvxwd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/guolzncpy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gbjxwiipx.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/giykkhint.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gaissiklm.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gpxhshnrv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gjofryuke.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gtywgewvw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gdgpzcilw.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gkmarzwkq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gwsmrfxsk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gvuabeezo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gxxjbavlo.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzoxiqkfy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gfymphwbi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gsihmxtgt.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/garicxftc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gbhotcpbb.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gduvghypg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gzgnxdwjt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gykrszdfo.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/griflkcej.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gczdcaeys.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gjexnytkw.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/giajalrvo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gvxhvvlwv.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gadtmcwxz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gvhhapbbb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxstthh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gguvvqsro.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gvomkxeks.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gafyjeynm.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gpqgxflbf.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/glgkalfab.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gonywbqcq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gvfscjitv.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gcynshzpu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gfgploxmw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gsvykzduq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gtxxvobcf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqduwyrxj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/ghbreunqc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giezlpqak.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/glfeguwus.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcommbomp.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gfockdwud.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gpsiwilrh.sHtML


<!-- 参考信息 -->