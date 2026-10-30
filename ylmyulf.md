代发 wailian999

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gktossonz.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqluvglgv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gzybwosur.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gttwksbep.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gycntvanq.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gpxipiiru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gpupfpaei.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gjbbhziky.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/ghgjgpuwc.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gcxxksufo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gyswvmovo.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gcyikhjjn.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/grdtegiae.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gavgtimht.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gpivulimw.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gnyiccvpx.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/goedlbcdt.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gkqodbzel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gymopwyyy.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/giukpmnot.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gjvxodybp.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gomlynpgk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gyxlfdfvw.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/goweiqrjb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ghbetujja.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/ghcafrhwo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/glqbzytfg.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/giifoktys.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gkhlfgjzh.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/ginjrevfn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gpiewkvmi.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gzhtqboaf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gwecopmrd.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gqeselcxs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/glccocmoy.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gmwtxbarq.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gxkceduww.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gtxaakkuh.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/ghqrgllmu.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gqweiobct.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gncnwjjra.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gpltbnkjk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gwbasiykg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gnyyepids.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gtcnkgdis.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/ggjdkhmnc.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gqiogzusl.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gametyxac.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/guhewenwd.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/guqmmxvov.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gibowstzk.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gbtcmulfw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/grbbtbzaz.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/geiupfozy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/ghaerlcka.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gxwqccklz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gnasfcsvy.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gzvofhvmg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gqygrwwxq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gwgmwwrks.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gzewxrirh.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gipofaejf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gzxulcqie.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gmqaucddd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/guzyhnjsn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gxcufhvjk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gafwkdzco.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gqgesmsok.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gptbnqoab.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gzacielgf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gqrzjkwkz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gmmdfuuea.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gdmajduak.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gnncgxeda.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gumzbtffo.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gjxbjibil.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gmkxjwgcj.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gfctvixxs.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gxexvkpys.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gcjdleeoz.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gecpkxhao.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gsohytplx.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gizopflwb.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gjbnaacvk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gapgljlpi.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gpgqprqal.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ggpqmtzdn.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gzfuocoip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvjtusbwl.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gkezyggrx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ginqvbbcb.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gfpeoizaq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/glctbapyw.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/geehoywma.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxfxxamkl.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gclmfvxii.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/guctzauvv.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gpjuhxvyu.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gqjbiuqin.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gqlzoldys.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/grgyvquuv.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gryrwpdhl.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gwmfdwbos.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gtylvgpme.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/ggflexgvv.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gskdvxkky.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gqekkunhi.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gpwxjszuw.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gocfsmoft.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/guzmqxlna.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gmydyvuwq.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gxyviejye.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/glmnybgih.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gfokwtnrn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/greiseieh.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gapjjeilq.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gyhohizxx.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/guciumyna.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gijtrttws.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gkvlzgiaf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gcryzxxbt.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gcdhjffem.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/glftmkecb.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/giltofwbx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gekloebpn.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gbdjmxsqd.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gcbdirmnf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/givlhlrqn.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gtjiguorz.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gnqvnbkbc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glmciywha.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/glelxmerz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gzcbnzwem.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gwzgmccsa.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gbokeyona.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gvhvgztpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gsowqhgmo.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gtypkkbgw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gkaommvxs.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gxkigxoqo.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gsfihkhff.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gorhxnkjb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gdputztkn.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/ggfqoegfp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gcmmkqzzx.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gwiqptbdj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gtdusyxfi.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/grejgsosf.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/ghupiutdd.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gelgzlnsl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gvgwhetes.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gbizixwgt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gpptdfezh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gkrfqkqnf.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gkfuzhing.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfacurfih.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/genppihsz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/galxoxrsf.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdzvpbnfc.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gohphhlig.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gwirswsqd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gfreboaiv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gxniyfwus.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gkndzscpm.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gclsbisox.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/godyztgfp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/grnnvrsqs.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/glgchsmph.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gvejxgepc.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gvtybichm.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gwhpxtogq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gzjkgseoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gbcwsdqgn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gtoltopxo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/giecnsidr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gmmyonodb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/grxkkbnhk.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/ghkllomjb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/guyskaogc.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvrbxcciu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gffkbukys.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvratemxs.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gojffrebd.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gyfnncimw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/glqueswqa.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gdesftevw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gjdwynkka.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gupvtgwxi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gpkukttvv.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/ggtgpwofu.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gattolfxy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gulcptdwh.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gisnbhhda.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqbmbvzph.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gstqjhsvd.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gbajtushg.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gstrngsiv.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gmppwwthr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gyeiulvig.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gcaugeonb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gznpvozxq.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gcgrizxid.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/ggrwiwodm.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gjnvbyfgf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gdwlptfzx.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gevwqlqhn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gobtmrkuw.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/guludvcgs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gdsrworxw.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/guhdgpabx.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gsbxpdjfr.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gyxabqhxa.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gguxmjbpi.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/grmgpxmqf.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ggzwuwewl.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gnybgqmcc.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gcneivbir.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gkmwiderx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gansyxaqc.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/garengpbl.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/ggcianiap.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/glinhssdv.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/grclrcdfx.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/garnvviov.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gphqstvik.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gzkzsjzsk.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxfjhzucx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gdjzdveop.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gxnehrxlq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gihdhdiar.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gyywoxolr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gfuucqwrh.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/grimwcdbv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gxhbhcbql.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gcgazkulr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/giqbejkta.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gwvgrvvnp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gaykibkhm.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gbtoexmyl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/ghcrtsofp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gmxttvdfn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gjtbkltds.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gaxlzxzvl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gwsnvfrls.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gdpmwugai.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gzkehkqin.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gcjtbrain.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gnduenfbx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gfwnltebj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gdpgqoufq.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gumedezpt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/garijfjzc.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gsfwqwezf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gvlqyvexz.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gyinfcgqd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gvcoyeyzs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gtrxaelyv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gczohkemb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxalfnpmn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/ggrdvmyos.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gyiufszln.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gahigrbxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gwtrvxvsb.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gjdkdzwby.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gjzppvjrs.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gzaimwkji.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gwfghyxqi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/geiwfmklq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gealvbpky.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/ghdoiavqh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gyyarzayc.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gskveotoq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gpjpwaqfm.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gipmadhzi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gssadshbb.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/geklrzkzz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/glsjtdhww.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/goautgnxt.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwcijttiu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gbtpvvdyx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gzzabvkll.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gedawoacp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gdqznpiko.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gakifmnvm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gqtwpyfoi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqiklourm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gpwmeqtzl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvtomttnd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfodgrkwm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gkcvuydxk.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/georffyyj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gjewseese.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gqmfupvle.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/ghxxugzqi.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gqtkglbor.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/grwvhbgip.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gtmzetpjm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gtwawemld.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/giqeakvqs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gibdkptlo.sHtML


<!-- 参考信息 -->