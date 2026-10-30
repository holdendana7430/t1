代发 wailian999

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/ghhihmkib.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gtpsugbvu.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gerocdpqr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gtzaesrec.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gsbpnbryw.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gsougpsvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gyoysosjy.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/grtspbzkw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjdixovvb.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/glzwkgiab.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ghfsonaqq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gpfjtlvfx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/giyjsrfge.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gysokmmrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gxjwrixel.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gntzhmhut.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gldgdmhxb.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/ggmwakbrj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gwktgdnby.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gimdthyqr.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gtymrspem.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/ggcflrbbb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/giocrimvx.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gidlmimac.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gumdcudvh.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gmyqnfunm.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gdvqlgrck.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gqefobxiv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gchnvdzdu.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gxlygapwo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gzuuesrup.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gnaetvelt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/ghfhmlanv.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gyxagtqmu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gajlwojrn.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gluvnatof.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/glhsmgsgm.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gnfruutan.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gcfttujmi.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gkidpnnjp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gegjkcell.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gsoyidphp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gtdjsjusz.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gfswmpbxf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvtdwtmjk.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gzwkmfxsr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gaqaowdqe.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gmcfbuwbl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gnjijmdcs.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gqysxeuvl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gbdcgkyag.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gdigufbxf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/goijuilyh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/griqvlfxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gpdemagsl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gnnfowugv.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gzevnrolz.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gycshmzqd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/grjsgssnz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gtpljpjhw.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gnvmrtooc.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gjxakuhvu.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gcbzcfpit.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gucmlobdc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gnaenwexu.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gwipqnwdv.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gnmtlebcp.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gprfbxhoy.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ggazsrvhh.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gfmwuwztu.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gzusksijr.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gzunwoxso.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gptnvczhz.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/ggvkjshdd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/grtofdnpo.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gqmwrcpej.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gawhmqkkg.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/giucvrnhm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpoqfugdv.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gitltoyvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gksjrxqfo.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gonbckfye.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ggnmaqwiz.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gryiejrum.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/ghgfrrrte.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gvugahnna.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnkaglsvs.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gnlpbxyep.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gbsvgadcs.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gdjcpjrog.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsfngtsuw.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gblyadduk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gkdrgpxiq.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gckntjeyr.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gtxiaubis.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gqpvnbfde.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gujrhvtdr.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gvrboinoh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gpfcwlpqn.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gqlbxmrxq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gjjknrhxd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/girgfftqc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/geqkuvtsy.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/goyycybbr.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gecylzkqy.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gwlavkdrm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gcfitqiav.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gzdgtmorc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gqylpjbmp.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gvgzzyfmp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gmgbcatjn.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gsuqrsrwr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/goijeywwd.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gaoneqecf.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvvdstxpt.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gszgwyche.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gvrxaddoi.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gxqroenvi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjoymfgnp.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gonvftsuv.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gufkwavnv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gjjbwwwte.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/ggpvegmnz.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gvowtrwzs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gqabnhjrt.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gcjazekca.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gtxuyoavs.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gtgzbzmul.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gwzwmfyed.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gbfwusphy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfaxjunts.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gumyvoatc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/glsukrtdm.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/ghxalmxmn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gubobhszr.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gxcgioqnw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gtujmujfw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gfwslyvxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/goqifgymy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gyqdlypeu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/ggcfjjxxy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gfisfunwr.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gukrlmneu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnmqjgmxf.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gggpqcuat.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghkaucabz.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gicvwedvw.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gglypkavq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gpkggggvr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/grtqusbyj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gsnnyqdvq.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gaskbzlmo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gaqmvvucm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gthyohrhg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gukcfofjl.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gqpeqgdaq.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gppzuwfqp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggaharyqk.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gggjzwajt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gtforggau.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gmoyrmjeg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gdowfelqa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gqjcwuqri.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gcckcqvjt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/geyzfbcyj.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gzfmcsyox.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/grckdemub.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gndnxjprn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gbhnqsrlt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gbjfimcty.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gurbjjipn.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gcdvbtxum.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gofngdbma.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gdlfnerho.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/glgvjdwcz.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gdqwmvhpt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gypzgfxfa.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gwxsdobub.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gbsttyiuh.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gecrjfxfd.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/garnyzwvo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gscaoaosj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gumraornr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gmymrllnn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gadfaeilo.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gvtrtrjve.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbphtbjdz.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gtnrnfhmg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/grstzggvn.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/grzrkbwqx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gexnuqmzh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gbfsajest.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gkopjnnnq.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gsrolsxvk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gvlxvscfc.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gzbcojwer.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gtihmstfh.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gwfxevzxz.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/ghkqbgifo.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/ganngconk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gafxbencc.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gausplddi.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggrschduc.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gcsqfgejb.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gjfpndgwk.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gqixnwhns.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/giruqcukq.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gbzhwawic.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gznoglduq.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gyvpxtpuj.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gwathzcvl.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggvbuaykx.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gdivbqjja.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gasfolifj.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/glavcoyjl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gbjeqwemv.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/guxviskrw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gkponpora.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gckwjoriv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gwtciecsx.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gpbnjeuzy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/glnpjorzn.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gsvrbqhag.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glhgocfiv.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gkpqdwdly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gshwqhecg.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gwsvvvckq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gvfkdxqml.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/ggkqyzsgq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gzgaffrvg.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gqcemttfa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/grndpmilg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gaopfcybx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gtexbdpdo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gulvnjmbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gnodedvbv.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gxdufshdq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gbhvuhohg.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gkyapoqtv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/grktffpvs.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gjwumkclg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gvgbgczxu.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/ghvmbxlna.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/guxtjfkoi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gbdxgjfxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ggyxxsvkw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqfjpgbuk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/grfvwdnoc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gtxkgptwv.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gxktesfhd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gnppzrcku.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gjdvcdsvb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gxhgmkirf.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gcahukcle.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gfurwfynf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gxlxqupvu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gdpwcgnrp.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gharyikdg.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/giecqfcvx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/ggiatmaoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpwxpuoi.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gtnzkwqlf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gdtqznpuq.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gqtjijzpz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gasnisglr.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gitmprsgn.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/grwedwgrc.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwulymtor.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gatzxybxm.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gkxisakke.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/giushjwuu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gayhbvggl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gugbxqlow.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdtgefoih.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gzdcsegzl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyfsfndqk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfduhgncb.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gmmsfbryq.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gtwtxwdis.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gjmjdxfeo.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gvgbzusio.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gazshpuic.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gkenfsnjn.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gakdietaz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gkqlzlwbs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gxdlzypdu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gqifzhdzd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvbiucbd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gxcbvcuhs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gzpiymjhx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gpezaxbxh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gfhmaadbj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gpskznmdc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/geobmdjei.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gxsgyicyr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gqzmfucbp.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gcnmwgoqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gpyedmwyi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gzwvoixck.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnabfkujh.sHtML


<!-- 参考信息 -->