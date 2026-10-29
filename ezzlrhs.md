代发 wailian999

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gtrrxmqad.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gnfzdriri.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gvdsmesix.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gctfttkrl.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gfaqjygsq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/glsnwgoan.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/glgiiomiu.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gdqmdceno.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glmrcclmp.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gdestawjz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gnpydzgis.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gkjjrmxha.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gqvzfnzxw.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxyafzhwa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/grdesdkmz.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gmyrmfdkp.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gbxyuhjsy.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gpjbsrhqp.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/grcvsevpo.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/garmjbolp.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gohsdeenm.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gqryolxbv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gjciafahe.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gofgnkjwz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqqxoaclj.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gaataiaqm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gnmoloszv.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggdtenreo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guiceifbt.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gfpsbpxoc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gimzykfsg.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gehqzyyeh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gmhovgxfr.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/ggecsclyc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gzkjqipmv.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gindhcjkw.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/glmufmsop.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gslwslosq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ggpxrkkbe.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqzbmvqur.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gspejlbur.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/glmrxenxz.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/geoxmrwxz.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gmhcntnmx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gyrxfpryu.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gtidswrvr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gqhgghdhm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gkenlcpcp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/ggeibwify.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gmpnvloxz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gndvqmvwa.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gtsszyarf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gvmuefmif.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gimrifafx.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ggnfvrump.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gwvnzvwss.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gzhphwtsd.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/ggtdqxffk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gcefgzdvf.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gsqnapcmk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gonaasird.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gfqegwgwb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gnoorfywm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gdnavpjdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gphvzudya.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gsaifutsf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ghrzhfxyr.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gdcpwoqqe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/glgiruvmo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gmwisvufo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/grfrmqqce.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/geiuzigdz.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gainbwhcl.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gdmgyuagt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gvalczveg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gqifwbwua.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gfvclfztm.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gavvolixt.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/giyyxqliv.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gxpolafap.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/geqwmvbgw.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gchjkjnhf.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gdyiurogz.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gceihxxvk.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gcztqnntd.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gnvnhxbeo.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gssdkiflh.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gvmpcqrqk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gfjhzhvrb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gstrfvoma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gpkteiprc.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gnqnvfavl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/ghjsjvfnv.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gkmmsorjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfmarpses.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/grrghgbnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/ghqoavjsk.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/ghgrhoabq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gejjngesw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gxeuuxsrk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/grrsgmmwz.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/glhrlhzjz.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpultgjmt.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gfmndnuaw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gugynhtrs.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gmsgwtlzg.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/grlhqoygd.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gdqwsmech.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/glfdpfist.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gxlgforai.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/ginfgbmxc.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gjubythkp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gmhvbvvfo.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gbuopvnpc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gcnuxdjax.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gzchpqbhw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gcxrqhnea.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gvdshywyd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gldfkuwxx.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/goacoeeyb.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gmvubgyse.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/glyfdhodj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/galzldkrd.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gnmsoonzs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gggdxlkve.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gqvkdaevs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gkzghnwqk.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gcqntbujz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gleneqhzv.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gckwyswqk.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gmflzqlwu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gebivzhiv.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gzanzofra.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/guuobtngi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gibhwkkse.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gapazivtp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/grkiaukqc.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gyuxegqui.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gcwmafaxr.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gkdcybgko.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gokjfwvzf.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gfutcturj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gvbrrghxr.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gxnyrpdbj.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gpshsxbcv.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gswqblrrd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gjiklkxkp.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gtkgqotpo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gsdsuenhm.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gcfqbovzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gwcksqrzj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/ggvoalxou.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gsiutrogy.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gcwtwkepq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gtmigljom.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gicejykca.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gfdwkqvlb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gdnvtpdle.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gedsbbgqv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdqkydxfd.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gquowifyz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gthjtrznc.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnbaoysdu.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gpurhsfsy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gepxzpsjk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gxfxwyivt.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gqhdzmwgo.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gsmsaiokg.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gzezykngt.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/guvvuqpqx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gcrlrmccd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqhuzou.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gfnvsrijg.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gdrsfujxs.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gelcbmdkp.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gnnmryftu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gxfilsvxq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gailfbbxy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gabtjklkm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gfexcvyrh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/guzkakjbq.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gvmqficfs.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gttynmykd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/galhujwul.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gxwszaxms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gfnqujvco.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gjmywuowd.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/garxcqlgy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gvmrskikf.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/ggelvfkpx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gnrobcprc.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gouqwegqr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gobentfko.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gjeocwdgp.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gwrlwkbnp.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gxgkmgklu.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gucvipubw.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gfyugqlty.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gmnamxkbh.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gzcqugrfr.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gusvmthaw.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gookfyipe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gdlbfvozp.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gabonjgfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gmfccptss.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gnrakvwle.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gjdcjwoaq.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gqptyjfxn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gmekqkrfp.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/ganygzwah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gvjafggui.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gsujsghei.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/grzmukgtk.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gxfcfyrsr.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gecqbwhvj.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gwyzecgwr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gryqfsprl.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gottpwqen.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/guicnwjic.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gjlsgfczd.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gvsowtket.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gstjdiuro.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gkjhllzmf.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gaxhpbmya.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gusvdvwes.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gdqakjjgo.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gozbymnhl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvojkkatj.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gpuihqnfp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gunsmiegv.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gmprflllx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gbsvducrf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gjblkcyys.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gwaiclaqt.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gvgqvtspp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gaibdzduy.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gswiukquu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glurapagy.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/grymaawao.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvxcygquz.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gwghpkjkg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gobyiqqyw.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gogtbgkjn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gioqrgwpe.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gzhtmmqnq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gtgayfqiy.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gfaunwvin.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gdkntslbi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gpmiywhrl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gmuyloqfo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/grxbugwxa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/glywrazuq.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gfoakeiql.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/grdaqbevi.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gohsuipxi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gmngrfrcq.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gzzddsxqn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/giqycbbzy.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gtvuoywkn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gwagqlujd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggbnkagqa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gmzbovxje.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpnjcslat.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gitqdpuwh.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gewzkrnzc.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gvmaabuts.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gawtlhdth.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gkugcptwp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwnfugfnn.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gsjsoourf.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/ggpqroovt.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/guknhkrxi.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gnazutiew.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gzsvndqsy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gadugzysf.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gupaxssln.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gzkepnupw.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gvlodgddv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gxkzadhhb.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gbhysegjy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gaboqebxe.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/ghnmykmtc.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gaflzuapw.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gmnuyfuvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/guaygqpwu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/guyookiiv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gurgdexfw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gfmggsvys.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdsutyiir.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggdihnegn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gpytlcjts.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvxilvfdc.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpqufpryh.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/ggkenmlhe.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gqngyuurv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gdureedeg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/ggktonkhc.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/guhokgyjj.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gfpynuuhu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gkdxlosvw.sHtML


<!-- 参考信息 -->