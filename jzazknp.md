代发 wailian999

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gidgjxejz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/grtebigor.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gddzxgrkw.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gmvcxmoqv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gjstypttk.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/grfdgglrs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gocptminp.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gtpwjkidc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gdpulpaqo.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnsknceea.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gepeudeio.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gnerzbgag.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/glqbrykxw.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gedmcstbh.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gvbdrslee.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ggljughmd.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gincabjbf.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gcjxqazgh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gsnclbypd.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gqgtvefcc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gyhmsknon.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/giboyoias.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gcborngez.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grzotzulh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gjewggvjx.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gomkwawfd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gnuevswzc.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gxndvmyox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gdbbirifr.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gixezcaph.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gluypxrfb.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/grhbjbvzy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwvnlvvvz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gzyxbszpb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/guuulbpsy.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdrtrwdis.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/ghrqmprjr.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gxmbksjli.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gxzdzumbk.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gifzkvsgh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gcfrbkdcy.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gxsijeeyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gptuivgho.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gwfuvgohs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/ggxitclyd.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gpaivtgja.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/ghkmspnbc.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gkdxpylvd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gmmhdqfzs.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/ggoevrujj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/goypnmmrx.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gxjyyfyvx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gozdyetau.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gecqfuobd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gbpwxagwt.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gneljaiat.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/glfoepseg.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gqmvgadzy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/guiutffgm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gvgprzzip.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gwhtnlbrq.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gdgidsmct.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gfjjkdsxv.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gjgzhfvox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gkljtthhz.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gvjnswtth.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gdwxrvejk.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gvnmjqsbj.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gjuiqxmci.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gutkebfgk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/ghbzlsloj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gemjvxvjf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gpcswgtuv.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gxgqtrrda.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gdeoxaxrn.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/ghpsgjgja.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjqtotlbq.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gvltleuhz.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwsrvynrf.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gaemqkksl.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/ghgwbzbbq.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gwsjcmynx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gwrygrgwk.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/ghlniidsu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gykdtdoqj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gmkifbtcy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gcvlasggf.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gogdloxwq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gihwhnhzu.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gjzydsjwn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gkypuyovw.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gzffjfxsy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gntfesfyb.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gkcesdbzb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gunspcoqw.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gdmktbqca.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gpkihwhys.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/grryxqdut.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/govonrjza.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gaqalyieo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gdxgdcygx.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gnyxgbvgp.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gjvxzgcek.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gbstzvdxu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gacodgklr.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gdowwdgaw.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gozrdtode.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gdfuyowie.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gioexzeat.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gwbqpawgt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gqghghjzq.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gpxcdzzoc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gaxhvneun.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gzxgdsdfu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/glgegfmpf.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gskazevmo.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gfqvmhvpg.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gyfathwkf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gmsmxrdld.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gnnshfwjf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gfqfabhbj.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/ghdeqvsur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gqgcaqkfw.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gqujffbxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gsvftibdn.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gpmxjqirl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/grsrcalcn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gzfcromie.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gsozlgjay.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gjljqmvsb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdaqaocfh.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/glaihvzuh.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gwnmqsicg.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/ghlzlbzqd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gzekqozud.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gaypommjc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/ghfmlwsoa.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/ggusaylpr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gslqxbsmt.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gnjetfgxg.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gmdhcvljh.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/ghqoavlcw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gltqxvvhw.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gcwkabfcr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/ggwxsicip.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gckmcclsr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gbgjxojsl.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/giokiehcv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gmkmlqyzq.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gyyjsmgnf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gfveybtfu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gbhawgmfo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gqkddorsg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/geykzcwmc.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gydigaxow.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gknjstlbk.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gosrzkmxs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grdyhudcb.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gnjxboumb.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gqlhijwgv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gpprifntl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gxpgiawcf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gmnlthwrm.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/geicxkqci.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gtiwkmbra.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gvnljibdf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gabluwujp.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gmgamtoss.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcqsvhmtg.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gdpyihyid.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gomrxdpzq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gcuixvubt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/grytlrnzb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gjmxkdnnz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gjspwjoma.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/golnyxtuy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gebdcewxv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gsqqljwtz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gfuvecvqg.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gwsvcvrhx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gkzucogjz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gqqhwfewg.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gtdszyobw.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gnchynfkj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gommnpxrb.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/goplvhsom.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gsipvvwfq.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gcdzcuokc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gyuilgqvu.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmsxanime.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gsztkeubp.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/grqtcacja.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gnlgfniof.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gkonjpbuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gihksvqiu.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gxcjuvbbd.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gmoozkkug.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gsvnsichg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gtazmbtxi.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gfpsbphhc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gswheqdmi.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ganvittkh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gtpftjhjr.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gilynpipq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gmvvussfx.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gwholjdot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gndhzltgn.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/geckhqgmg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/ggqaoeros.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gtqxedzmx.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gclroiula.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gduhnaglf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gcpcbkdek.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gnexqhcss.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvwyajejz.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gohjoxpoz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gbxitqbcr.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gdrtccndz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/guyqmkota.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gxrqqvbuo.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gzzxdylpp.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gphktjvqg.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gmbwrbxhb.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gnwnsrzwy.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gpnrjbufw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gaaiacxbz.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gjztxuzdl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gvdwvgozk.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/ggnlcwiqk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gurrtgeuc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gdfcrjalz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gmrzvpcxy.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gwkzcodog.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gahpgrpxo.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gsybcyhgz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/grsrvdzzs.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/glghihpac.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gllwexmrj.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gfrylrrpv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/guwtqgvzr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/glvrkbkrj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/grzhblbtl.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/ggpgpdgjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gqksgjddm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gylpyrkyf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/graurdxyc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gqpmdwstc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gytfpwhkm.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gmndkdnrg.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gkycfyiuj.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gizvwvcdo.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqcbmfydp.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gfeiqmhwx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gzorptovz.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gtmklqeoi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gacrpzhov.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gauuarabx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/ggjdfkvfw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxlyuszyt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/groceczsm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gcoaphnby.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/glmzbvije.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gboijsrvg.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gsmleetqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsqjcfzdp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gjyvsuyqx.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gbciuochg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gcbolhufl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gmilffaxs.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gqeneozny.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gsrxfwsrt.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gqxijquwf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gshrzjfxj.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/glxjwpckk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/ghuaeanyx.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gcloskyeu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gtwdfbxtx.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gkxhaoyrq.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gxgryzffb.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gfubvjmnp.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gzxjvahmm.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gofsemjfo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gtvvcwzww.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/ggxqtnnmw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gchagdvlf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggfplrtfy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gnvbvtifj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmyqkvoar.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gezeenevi.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gyoqzpfcn.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gtdlkufet.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/ggxcurdzs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gwqlrmoax.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gerljlxun.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gdncuysko.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gvpidjqau.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxhzrcjvp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gbcrjglns.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gejsruuro.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gteyiqcor.sHtML


<!-- 参考信息 -->