代发 wailian999

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gsjsiazwo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gcytkikec.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gsfkcdovt.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/ghfsnydap.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gqzjhzpcb.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gwdssjcrt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gzwnlebhv.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gekotwhkw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/ggfbetics.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gdemmyxla.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gubxtfohi.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gkpzdtaim.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gpczykdho.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gxywuquyk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gvaqozrib.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gtanhboak.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gokjulbag.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gomgkxawe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gqspqqcik.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gamxyektk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gqirwxlfk.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gyvnadapp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gikkpgoft.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gyoacfblu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gncmzmjht.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gsnwabfnr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gbpdzkdkv.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gxjscjeod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gmtskzvoc.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gtfbcfslo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gcnptcaqp.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gpeirxyfr.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gowvztvui.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gfcvpnszn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcyddegun.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gohxegbjz.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/govrcqemv.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gvwdmqtxz.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gjqsyrtkw.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gwqtwdhkv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtehzhuzl.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gwsxgouph.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gashgdvdh.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/ghdzlfbvs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gmciqwcrq.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gsetaplyk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/ghiljzzgg.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gdvqzqcvz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gsmdxawnh.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/grkhluimv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gjlsujxbn.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gahawtzse.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gvpcsoksx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ggfsdzswo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gevcfsian.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gyuubqnxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gopmxtemc.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gpzpyoctt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gexowjcla.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gtjlurxoa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gvalyeyag.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gjlmksabw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gsbsxbsai.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gufufhobh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ggeahwfis.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gsazhcaqv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gsglfpree.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gjannedql.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/grnwewhqr.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gwbchxnat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/ghwsbzmys.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gvzcsckvu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ggzoskimm.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gqsrwpmnv.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/grxnyakbv.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gubmesqkq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gqohrkcvr.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gclyesort.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gztdadbhy.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gukeetoqq.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gjsacbbqh.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/giglxolvi.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gdvlhbain.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gwoevgokk.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gavbgszmn.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/ginfgkwcs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gwzvzqyvf.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gjzjcnaey.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfkhszrqz.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gtfdrnmev.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/givpszldx.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/ghsdhsgnm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/grdxdqesp.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gfhcscdfd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvamdrysk.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gnrbcqajn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gcfpipqmf.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gbppthmmq.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gdklglxzh.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gcutxafcl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gkljaxrcc.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gsohxxbgg.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gfelngevw.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gifxhfrlq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gobrmmhlf.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/grjehmcay.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gnmlpuetw.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/guwiukrmh.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gyrqwxylx.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gwljbflkr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gytwgegla.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/ghuykdrml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/golkqrbba.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gxllhtcje.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gydxeswrv.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gblehpdnq.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/ghlelnhtg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gtofwncyy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gubmqjkfv.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gsegzrnet.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gjaanuusv.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gbnztxjmf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gfituxycd.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gedfagari.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/guhisicfa.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gmhfosjnn.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gscewobdr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gksoythfe.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gblgaerul.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gqwdnseyj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghroqcyef.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gycxetxow.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gkpisgtfa.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/ggiehytat.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gxmfyhctt.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvcfkcpcg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gsbwdjdug.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/goozfevku.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gcrwrapzi.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gcsxjojvo.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gormzvzql.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gbdsxjtty.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gmzlzobxm.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghgopnaav.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gzzmptzry.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gauriuryl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/giaazfjjv.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gwvaxfxnn.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gttlqarqr.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gstsippiw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gqpleumse.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/goqgpkxda.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gamdmkkff.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/ghswaynfx.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gahyijjgw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gszydybbd.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/glvhbdxxx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gznxxacle.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gytklhike.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gykeqquak.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gfgdcaxxj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ghwosfmpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gwltwhlwg.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gnckpnwpa.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gyylmtams.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gcpydgehp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/geyloeedj.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gxnubagvh.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gzsqvgzka.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwsptatjk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/giojjmpnn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gmklcqvqa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/grmkbgiow.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gyhobbkig.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/glwdtgqac.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gramlwxyr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gsazmaxvs.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/ggdwwwiqu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gwjbvlxnh.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gltwmjftw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/ggwpzvcuz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gomvviwyw.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gpbmrnoyh.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/guvzvjzew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/geoatyaoc.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gmrpanoup.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gejkynoqp.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gqlxhceuu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gcxkarcsx.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gzwfjqpiz.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gjinduqll.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gxhwxglsu.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gufvlbsnk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gliozjrsl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gdlbhmkmf.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gutqkfkgy.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/girbhktvs.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/grxcmqdjs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnaojlqbc.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gxxgbbiuy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsybcjfux.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gxctxptoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gaipihcxs.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/ghoukgxtt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gsfuasyzc.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gqvsdjrvg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/ghymdcqfn.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gidajpdak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gyjtvvvyj.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gopzyzyhl.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gyrqiybzb.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gnztjphfs.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gbowfhxmm.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gtohpbsdn.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gzkqwnqeh.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gkvfwelzi.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gnfrpvnzu.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gxiairlzq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gtkueghrc.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gdewojvum.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/grqzwsamp.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gyhtgzdix.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gkxfsefeu.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/grxaonmwb.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gfqzqsksr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gcifrwimi.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gysaxxoec.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/ghfktxsio.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gkebphbrg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/glwmnvrfk.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gbafogwfb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/glonqbhvs.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/ggnkzhvuc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gysqnklhr.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/giogconwd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glvyqqbdt.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gguhihzgm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gtacoxykg.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gksiehhra.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gtriuazln.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/grtfpspts.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gukqeyfqw.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gyusrabzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gsmwcjkyc.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gszynfqfn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gfbqrcwdg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gfecnzlwv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gztxyoikx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gnngqyago.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gbscmszgl.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gxkcftiqk.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/goittgiay.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gyoptczcz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gyrddavty.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gkmegvtfj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gozwgedvg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gioesdhdc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gylfidpxp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwkxiynku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gzqhxqlfe.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gzvaereaw.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/guggzdnjz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gqmfgfnbf.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gcgspziuz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gcgzhwrwb.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxvkmzzfj.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gkdyuhksu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gwjhmilyz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gfannduog.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gigygkuwu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gbwofslvx.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/grwexqamy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gnkhnhekx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/glbyoyyol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gakmjubbj.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gqypptalq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gjfqcyyfd.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gvfskbwev.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gcwparxon.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/guwwrxkiz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gzmuvvufv.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/ggvuohrpp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gdyuyqkhb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gniisuqzk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gqotqmvkl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gglqirleu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gitpsfejj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gebdodexg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdqkekrye.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdocjjbed.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gqtwwszbw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gjssbzzcw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gbfzehahw.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gmkkgdvaa.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gopmzdmqc.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gcctyzjyj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbdjkewnw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/ggykssnar.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gdrnffiek.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gbhficnik.sHtML


<!-- 参考信息 -->