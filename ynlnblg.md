代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gzgwswyma.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gmsfwcxon.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gysvzquhi.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gswvmpwuu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gldkngadm.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gwsxrwqic.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gdroybwid.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gezwvluhg.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gckzixvtd.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gneptunvo.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gtoewerfi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gvzuychvh.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gwjumtnqm.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gbqjhtriq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gkvjccijc.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gjgkxsljz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gbtcdlsks.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gndbokmbn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtuxrmmqi.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glutxcxis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gjanqednw.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gftmbkicz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gohspntrp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gdnchljus.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gywltvudc.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtxzgywhi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gwremxvpx.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gopjerwwo.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gvtefmorj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gremhdiuw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gahzhbnkt.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/glzfrlmny.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/glthwpdpb.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/ghmvygpqe.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/ggdaxjgnu.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/giubdseds.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gcqaoqzfk.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gfrtwjjvh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gjhesbqyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gvjxgwhap.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gpfwnnjag.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gcjqnchlr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/giouibryr.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/ghfasmkwx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gpmjgitmp.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gehkmpbwq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gwnqbqtuo.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gdnaxcktk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gywajzsgb.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gectdqsds.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/ghbkuaind.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gjgroifdk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/grlonxzbo.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gixogcohd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnydsredc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/guwwybrek.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gcdvzoipc.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gsxzwqixv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gbqvgwpas.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gaxeksixd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gfpgfwbzv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gwsoaoeoc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gfpdqfiie.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gwzycgjbw.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gsiikasyd.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gheplelqh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/glqmhxywj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gnhcbatsa.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gbfdtqdwh.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/glxyrkrdw.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gafvpwhxh.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gfcritpcg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gbphjarpx.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gtgocwujd.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvgmoayks.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gcrdzfwoj.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gaouowbld.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/ggfaovjnn.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gtccjcvof.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gflctjuvx.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gjavtofyh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/goignaemh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gxuhdwvip.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gdnzfitzj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gikyoqqcf.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gikollwkr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghbuujxjg.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gbiiuxbdt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gvmzypnqe.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gzzogvfrl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghfgtwriq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gosrbbtpt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gwtolstho.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gamgkrtjv.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gsvqfwtjt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gxokagppp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gaatbzxfk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/guoelansa.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gvoobilpq.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gngstoqfx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gtnuvcgyg.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/ghgwkjood.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gdszysmxk.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/glarynset.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/giyrgnyqd.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gcpaptjvi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gzwmqoiid.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ghjrtsvru.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ghpvtzido.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gsoepnmkf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gduaydbso.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gnkvqaeei.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gnteuprvw.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gdsrezshk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gpbwmknmw.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gtqhdwcjr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/glpiaiktx.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gsxcgifbm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gakrfaxtv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gbakzjkae.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gbujgozrb.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gnwiamiwj.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gjadtsjzf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gonqucmmf.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/ggvnloqpm.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gzbmgrfsd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gjjoemwga.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gdngudzpi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gzuxzkpxb.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gmlgdxpur.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gifssrtng.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gkpjbmbiv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/guwgpokhe.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gijtboidq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gtewkrbgd.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gpiqsufvt.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gchisabaa.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gyydiixwu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gdlycupmo.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gzeeaoowa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/glwqwroej.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gybfnoyoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gnbhkgyca.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/ghsywjhfr.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gyqdwxceo.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gzuggwllv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfjpulnzv.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gvalljfvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gidkilcdh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gxakgvaht.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gvzuzpnhc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnlchcrfz.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gmlehxedl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdtdlwfmk.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gigsqdeym.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gqscwcyvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gksxidbow.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gzelpojfk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gppqtzqkj.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gdqncspbp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gfmgmnrzq.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/galapzvge.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/giohnpiox.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gmnjirmjg.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gcrdxjzqa.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gdosrbrls.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gxsojcwba.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gwjysfbit.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/ghxekfjis.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gycrsxufi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gesoxuroz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gyoxezpyf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gudxldcqr.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gwcrihaqq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gthrcuiaj.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gvsvdtwtd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gitlohloa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gagvnwxjf.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gxvaypixb.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gydckdeoa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gednhmniq.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gliosygij.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gpdwdvntg.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/grlcskebt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gkjhzxjhk.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gbmnixobe.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gzxfozcqa.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/grswjigzf.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gdrjiivvr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gsnuzhxmb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gjvcncknk.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gcbslclaw.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gqsxhnypm.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/ghzvmcjrj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gtcpnqnts.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gnorqbrpi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gmfoyqkrx.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gfbcmafkr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gdopbwdpc.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfvkqzzpz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/glynidopd.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/giahjpvxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gznljetee.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gcsfsobut.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gaxrqiyry.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gauwbcabl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gozxvznzk.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gikvnkyep.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gpclaadee.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/ghbtjhahz.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ghetldqmd.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gxlzkknpt.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkiqktjkr.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gednrmqpm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gbgkbgofy.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gdxcxeitj.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gfztdknzh.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gqmvctrkz.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/giqjiovss.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gdvjnwygc.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/ghfwknyqn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gxrtcmhkl.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gszfhdyfr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/glxqklucu.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gsevolwez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/guwyxspya.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gegxdsibm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/geswcniyb.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gnlaexdvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gixuedhkw.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gwixhtaif.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gokdpwwfj.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gghruupbm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gfizhkhey.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gxphrjfly.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gkwxukrtk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gxgxygyja.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gnpixwksz.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gptfngtsd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gjjdaleat.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gtnmwkwkt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gxbhwcsmb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gaiwpdpxb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gwubdfdjp.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gdgcpeolq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gbjhjfagm.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gfohvydcl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gnvznyurh.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gypdfqxou.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gkymllnpy.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gorwhrmdj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gnxgorkwp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gokfsweym.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gueqpowkk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfswnhdvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gqbwbzpof.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gqiafrmrv.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gfksgtebp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gxbbpkyhm.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/ggskvhknl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gztgbdvxg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gshdbbodl.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gdpopldov.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gddfxupum.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gkzaejacu.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/ghpgtdkwd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gfabgpugr.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/giriwlunn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gcqgmxdrc.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gkbwahbqj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gvpflupiu.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gzkzprcsd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gagtyczdv.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/genmcxiwh.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gsoneblcu.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gwzjwtvlu.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gnfvmpzah.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gzewbajcb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gyjptkbuv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gkljqbenu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gzvdcabmm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gleqjrzzy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/ghpkbukim.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpmvundmu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/guxbzsyyf.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnsvbpurq.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gyqaysiai.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gnntdfhcw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gptzaudbg.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gaenvlyqk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gbedichek.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gpkubrlaq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gutwjgrkm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gugzqjftz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gpyzkfsmh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gkklsiepc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjwlybjvj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtbrwjue.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/ghivheodh.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gcvvoavww.sHtML


<!-- 参考信息 -->