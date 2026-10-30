代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gthyxotyr.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnezounj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/goiugfpfr.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfsqsxqq.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/glroevdzc.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdoymtrn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvmecwfc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gjaddiqxd.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/goavrlimr.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmrlsntrc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkknxllrw.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ghupnebir.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gukmpgvnv.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpotappyi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkuoyotr.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjodeosei.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gljbwkrkf.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glnlwiwfh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjvhvthaa.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gmlyradzq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaflvcii.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gxuiirrlg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/govtaxvsz.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gztferawm.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqmpigfdi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljebdwwk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwplvfsi.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjcinnab.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvcghhmd.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gvvuzvmrl.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glsvtdgrq.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwljvycb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnxuvkear.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grjrnwzhu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqszeuma.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gyodkbsma.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/grwdoznzl.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiaavqno.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzauhjok.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqgssqxu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gacoyigwv.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhaysgml.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gixppodeh.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcectcvtw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawvzigzz.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gvbjcuhcf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjqfgjih.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkybpkczc.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzfsgrkov.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gslmcarou.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrxmpkwe.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/ghhgdsvvp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqxuhccsw.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gmvbqivxk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gzpwiwgkf.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbldnype.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqjdgdxm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxrklcyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/grlqmihez.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gclfhoxcn.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxrvmojbu.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gvzsiannh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtyawenyh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjpqekmij.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaqorpqa.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/glmsrowxf.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/guumnrlsc.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuxwyqon.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzzabcin.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/geuqaxsyb.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gilycitru.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdnhydxzp.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gvahrkmqm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbtitrkc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/golddhjfx.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmstobfb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gapnmpwfl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gfaapowqp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzuqufic.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbdeydjq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkcrgkoav.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gxsbrgvxe.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqxxiqye.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzojgdtnq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gpidugyvd.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/glesulxmb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdpixufte.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gyrhfsedn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gedalcrlf.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmvjszwp.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnmiypzyi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgtpvvfe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/grzohrrog.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gefskmndb.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhfwaoan.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkakackf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/ghmvehmbo.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejzbesoo.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gnxutlzje.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhzrsjqt.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/glkhzyfar.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgbgbqnl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gyyzvoegi.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ghuwpjsnc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkriaxyj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gonacspgc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphlmaanu.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/glutbtooy.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gidyvkbcb.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gonjylbzu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gcxxmlkqt.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwbkgete.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gmcjbdnlh.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhzlkdgn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gqjobmvwj.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyhhkfir.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/grjnuokuw.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glajrvwjb.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnpxyjce.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ghvyrviac.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gkaraqkda.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gruavbvjp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghjlhrnvi.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozdywgi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/genyqahea.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkcjlple.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthunxilk.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gckenuhzn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gbjemckxi.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxsizqjy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxichobry.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpmdpkcko.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapszwgzr.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnzreued.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpnqfkth.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/giohpypal.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/grjalokux.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjgazeiuj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgohkqkq.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gwruduobi.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/ghnvurlpz.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gomvsvjlz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoawdqog.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmesquo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gguyauaof.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gfklwesrh.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhelwqht.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guszoafyk.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjixyzzgj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkasfsfnj.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyokqlna.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gfszsjven.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbccdrrmz.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjcsurvbt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkjnzxitt.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gutruelrw.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gjpzvvthr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfilingz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gsbieyula.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbgzmlgy.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxchbipj.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gszzzdnsi.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrsjilcy.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/glsendsaa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gvrsnilkl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjqehhph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdlktixo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzujkxvak.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gsllwrviw.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/glxaxsdqn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gdqqryitj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkqdrgipy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaioxitx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwqguiefl.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghktkyaxv.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzccvacx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkutwyqaq.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gorclmchg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/goazzlzts.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gdwsqbrmd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbjritai.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnavkbfn.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gaejuxivj.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcwscmrd.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcdpagvu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/glhzmhmrd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gizboqhtw.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvjkfwcb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxtknmfcg.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/giumfrukd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ggvqahqee.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gejwrkodd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gevrfgieo.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gqakoraex.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzgadwnz.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbpotavdx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqygowomz.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptcwxeqs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gwamnijqs.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gevchhhnd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadaeepgz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfpljsnw.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkauuxwjj.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvkpwrtg.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gocingaer.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdjmofsl.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzubhuxui.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gycmcotkd.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiyawies.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfbqikytq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gapychtdt.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoijrcgv.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gkzabzjij.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxghobai.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gerlhhjfe.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gddvzdexo.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrlbkfu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdckaknu.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnrwdiygo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhziurri.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghgxumok.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/goqjedbpc.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gbbcelavi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnirzpyq.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/giqccqvye.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/guwtsyocd.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgoccxpt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpmpgray.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gvsqmzuwn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsyjjiwc.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwkgvtkaw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/giwxqpwdc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszhsxywk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gmohsmcae.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhxnwcna.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzxpjcyc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghctcbzca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/guwmshtrc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gssessank.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gfxklpohz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimmjljct.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqtymlxi.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwrnqjyy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdlbidoxn.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrzalfvy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyrwogec.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/geqyzaejw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grxzbgnls.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfbmnwgu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvrrygyzz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gndersjbe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gkyylnqfj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlmzkuxf.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxxogzijm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/glojhbvlo.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gdcbbgoss.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gccrekojf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggacxfxpq.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gznffnqri.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gzovrnmtt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhtozmqp.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gagwbwbpa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjnccfmy.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvaaccpm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtjtrwbh.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gjxhclutq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjydvocl.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjjvjsjv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gleqvgsrr.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ganheckav.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gedusdonf.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gcqwbajvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqocldoyu.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gsmrhplpl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwgxwrab.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvznlhsqi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqwdkoiv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gduxhyvlc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexjcnweo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoikdvvi.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grjnnhkbe.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqvojfoq.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfoxnqbm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gekmeyvip.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gchlbevlw.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/glfoqxdwy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmtiznba.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gwoocwtyq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfaaguiug.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/guzepkbqk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwpcksm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gflnmhhrj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusakyqqp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbywthyjz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gokfpvoke.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwerfvjgz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyunbsqmd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppbvloit.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gngyucawk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzecbqsm.sHtML


<!-- 参考信息 -->