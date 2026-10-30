代发 wailian999

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gutarxrue.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/guuebqqlx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gumyomvxn.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gzeolozia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/grxbapyvh.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gybywcyon.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gsvkzakii.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gblhdiloj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gnsujyret.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/grkudhpgu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/garimyldq.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gnuoithah.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/girsdykrj.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gsvrrsink.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/geodsafqt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ggwpvdbqt.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gdeivrmfk.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gapshxocb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjtmdqzlk.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbtajzezk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ggwsodtwm.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/govdifsuw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gsoqxxthr.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gqxodrknd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/govlnszqx.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gllkrxzus.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gghffdxky.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/glcpgrzls.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gtydhdgeo.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gdemjzora.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gvsotkcev.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gmvcilmcw.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/grposgsmf.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gewefudns.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/guhgikzeb.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gfdvzkpez.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gclgxaoez.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gvmxxkmkf.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gunbgxdes.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gsfvlzwhw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/grgpjplmh.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gbcnlyfin.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gwjufdyvs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gbugzxqkc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/glibyggux.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gvtqkzgsh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gyrvdycgt.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gckohfhme.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gfiyojxjz.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gtdxficfy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gkmgirepv.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gcwyzovgu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gkvwvncxx.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gmuiobbpd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gonhgxlkm.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gdxpdlays.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gostvureh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/glvahjkew.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/glceatkfb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/geyizkybc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gkoukmljh.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gqmkfpith.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gqrddmkpx.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gwiksnwuh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/golgnnyer.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gfxqibgad.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gvvmminlj.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gyktqipgs.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gfxdruwmo.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gmozrfwbh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/greuaorsh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gzyzhuvxg.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gphtzsycn.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gamnbydqs.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gqlwzvmsm.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gtktndqpv.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/ghupobbfq.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gqpbwzfyi.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/goufrgdzs.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gablyfdxd.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gjiabmuqu.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gqsjhroea.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gpmedgioo.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/guveiphbh.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gbazjujjp.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gvgqpldir.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/ghcdikubj.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gjeseexns.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gizwbunkx.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/geubpkcam.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gxuabxpqm.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gwrhnhcyz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gulyasosb.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/garksdwvx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gydyhyhty.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gewxrlxzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gntslufgi.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gxntmbptd.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gevfhasda.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gkqpigoun.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gydfprojq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaytvdniw.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gakcevkni.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/ghtvptiar.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/glfhzqlxw.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/guwenicfr.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/ggqwboezb.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gzlmmkjty.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/grplndmfb.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/goljsnbiw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gfkrodipz.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gvstopbld.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gbiiddxeb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gwzdixxxf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gglhzyrbj.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gwicoihlm.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gdsgvimyp.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gubvculuw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gpmwjmegh.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/ggkqiwqyx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gbvixvxdt.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gvbqwywmy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/ghhikwjgz.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gtntfpeem.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gvcvwshhy.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gybanbhqk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gwhiwecbg.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gvrrcgnxk.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/ggiycrjln.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gjavqfbso.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gqfshsjlz.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gszcvnqhr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gwtgalujz.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gbsrkzyor.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gyecvsudb.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gkmutyplt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/ghszexnvt.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gjhufubcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gvexmapfu.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gwrlbvjsj.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gpofuahzn.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/ggzszsllt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gndozupgp.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/glvrujtco.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gwtutxqdx.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gckpxtudc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/guuubidyg.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/ggnbyanvb.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gqrfsopqo.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gdsgreijk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gwchjiihc.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gfhdnxvno.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gpwrhavqd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gwftgjhey.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gwpqmtbmv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqasfasdf.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gggdruodc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grwaszyte.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcvcftqht.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gnzzbwqny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gawbipymm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gdmegncxn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/giqazplrr.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gakriovlk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gogtgayty.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gnwvtskem.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gguxilrmj.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gynhbmdtx.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gzzbzgkzp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmfzhcqpc.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gbsvzfbpb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gfgeococx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gkspoyojx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gpeutqqwx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gjpuydbae.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gvofcttvc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/ggcvkseri.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gueajrhhg.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gbsqzetsz.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gpdgutgap.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gqomqnzbo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gctfnhkpu.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gjhbpllkk.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gsrvvewin.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gmyusjvbz.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/ggeihsnao.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gwzxbrqug.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gfcrkrstx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gmnqwxerf.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gwozcaxba.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gazkvgern.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gsblqcjql.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gxbrrfkra.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ggmuhmbjx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gwkxrlrjv.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gbrbvhksh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gagyfznbp.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gazeawwuv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gzdxblaai.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gdxlbknkz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/guaenczwb.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gemgqdvgk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gpqmpvlyj.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/grshzfnyl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/glxsvlply.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gtjdhadqa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/grwmdjoru.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gjirbdbex.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gzrizigrk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvvfxwubh.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gteqckalf.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gbchytcow.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gznqwohqf.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gpjlkfpkk.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjulxsdbt.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvwnnyeyn.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gdzsbuqpb.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gzlyukakh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gfirnlwbj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gbwdnzkhj.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gtvykjqlw.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/geygcbouo.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gfwwlvblq.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvsbkimbw.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gyhlevezh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gcziutckr.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gyhspbqwz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gpnkxetom.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gtnavynde.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/ghexgoubr.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/ghmetxtfx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gavamzxmc.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gqadseffa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdrmnsbrb.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gswydwxgu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gftqtqbpx.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gjbyrlrwj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/grfdjmqom.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gbqpwnobq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gnqidzwkg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gcbhaeqxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gobilgqhr.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gzskwukbx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gutqtuafk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gztjbndkg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/ghubkdslz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gluaftdak.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gnbegnpyl.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/glfcfiemy.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gefzjqmue.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gjazcqqdh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gkgbxtffd.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/ghhplndhc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gusehcotz.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gmlwfxszk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gmbikrrnq.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gsmnddney.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gvbnwtskg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gkyvkejhw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gkvurxxaw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gxhblwuwt.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gudvejakf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gdidwidcq.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gniqkmdse.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gljbhzovs.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/ggicqjnnm.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gdiczohvv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gmsopmffj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghpntnuyu.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gvfqmyxfv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtshfbdoe.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/golxrwsse.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gueivlzgu.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gdvjeosqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gufauhnfg.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gmkkhgown.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gmokngtxj.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gcxuqaglf.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gtfscrsph.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/guwtnbchw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gtjmuiznx.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gqmrszluc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gigmdwnbq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gjnmqgbks.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gcwianjgv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gojmjidbx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/ggroxdbmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwkelufev.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/glseaqxlm.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzutwmgdy.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gunzfacqj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gcqstxcoj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gataszxvm.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/grrqeladb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/ghbqckswa.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gofaxvtda.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gicfdktcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/ghkosydxo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/ghzdqorfc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gqxmcxpce.sHtML


<!-- 参考信息 -->