代发 wailian999

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gijtqemfh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gduyqnssv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gmweeoqgp.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gxcicmbly.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gsfosbudd.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gpkvyuzhc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gxceupewd.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gkfmytsdq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gmqbpulmk.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtrfzveiv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gouplsved.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gzoqwiqyd.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gpeykomni.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gbzndbrgc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/giqidlsco.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gvykehfnf.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gpfjmhrpu.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gyjwvgbjq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/geksfxajy.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gnpnmgeig.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gwokggqor.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gnzkyvvoo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gwyynfhzd.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gtzmsmpnu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gnxkjgggi.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gauhbysri.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/grhjjhgfk.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gwkzwfnnl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gfugtmznh.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcoiokh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gosqobvqe.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gtxvqiyev.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gvbynsmuj.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gpepunwgt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gkdwsruxl.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtbuwqdoz.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gsagegvsh.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gbofihqbo.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gpjiebsrp.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gkxamegqs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gahuxuimk.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gjuljegtk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gjemlvyfw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/glrntbpto.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/guvdjkpux.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbnelucnn.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gdmxtgwqn.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gwwtsbdtn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gnukzoyvu.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/goxspgxge.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gnsaxboif.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/geqbpjlwr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gloxxpzgb.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gvtidnngq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gqwizjgba.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gvnbipukj.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gqdvkrhhg.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/guwfvosmk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gdjqlhemd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gwvukhqag.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gfzasfjca.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gdaldfmcr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gyfadizoo.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gncmiuknu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gbivwglsw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/grfwzeqyl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/golfazchm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gnjggwqby.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/ghooyplth.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/givqobscc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/ghkvjqapn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gsvxskqva.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gowooujuy.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gqydrlwgp.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gfdrhxgqr.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/goiftbgre.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gtblsbmua.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/goxlxheyn.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqdxbebdj.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gbvccdvhl.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gzkmxknmd.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gbmauhwhg.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gjnihaqbw.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gcnvfnekk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/grvhadvcp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gksapphyz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gnjlehams.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gtvbgkcfr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/glmufnmyw.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gjrqvclne.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmfnbklga.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqkfxmh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gxyfwftvb.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gtswfldnl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gevyeqhyl.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gkvjjdhil.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gtgigqzcn.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gwsxgjejg.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfrxawjbo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gvqrirfok.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gcaaeabcj.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/glcywetjl.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gtxsndhci.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gjmcxkbcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gjxhkrbub.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbkfzvctz.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gdafigvnk.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gzdraptnh.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gffrxqkfu.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gxoizyded.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gdobsyoya.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqlhuiewy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gsiajcuaq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gbthwaqch.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gtilrhsst.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gtugjrtkr.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gkfungprl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gketyecpp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gqzflxlew.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gtvbeslnj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gbwbavyoy.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gykpmvivv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gmnisvkqc.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gymukfarg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gsmrrcblc.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gvkmnumhz.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gcpofnukw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gqujygfkm.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/glfaehdnv.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/ggydvhewx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpmhgzzye.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/godmedzgd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/goiszierw.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gtdimyxim.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gnqpbpkbp.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gpdddvdpa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gfjbjlzdj.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gsuxzlcmt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gtpeobcsn.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gdhpvsjoq.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gzsvwyrja.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gberdtfqd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gtkrsxnmg.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwnmnocfn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gmgrllztn.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gknrwmgut.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gbthosgns.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gvjdewwqq.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gateeimas.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/grdcwjjwp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gvzxolapv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gbgttfueb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gljroctep.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gbwnipucp.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gkjahaxox.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gikfqcien.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/guqcwotbs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gadzrrjdm.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gprnhjscd.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gselmxxmr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/ghvfdwnzu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gxwlehabo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gpkskchlo.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gaxcwulnl.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gmntespew.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/glsqlaqth.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gosybnicf.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gmspcinvv.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gcbyzmkop.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gupgecoyo.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gvwopucej.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gpkzhbguq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gxwscntgj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/grniocfet.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gmxilertt.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gkedwuant.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gklxpagdg.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/grcdnxrsa.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gcxkbjbuq.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gesrzbnkh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/grfozzqkn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gzckzaboq.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gxkbzdlen.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/glddgfayj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gpgdrxvhq.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gyokqyhpg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gyotrfadq.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/geonohspl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gnfkcerts.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxmfkyfqg.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/godcnpuch.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/glrqicuhz.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gbaivvrzb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ginmgmuyw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gbookxrxc.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/guziqnjdq.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdniqtmbd.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gjzpydntn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gghoxldxl.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gpeuazrse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/grcyeqbpa.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gtccbnkfq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gmepeqbld.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gpfzsnrep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gimbqtzke.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gkvjvgmsg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gynkyqmtm.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gixokrunl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gvqcrgdnx.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gielgctzh.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gpufsaesk.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gefrmynxk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gjdmsjivm.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ghejrgkgi.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghfxiqezt.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gdusxzsjj.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/ggaoirbdk.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/glvnhzpeb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gfdcncaiq.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gwtivofsy.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gfhvgclsl.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gghominim.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gkiopfvax.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gryvitvud.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gfjrhbqin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gdgnmzuef.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/ghjcurpeo.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gmefpcsep.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/ghjtubqoq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/goylkifbv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gdwpxhwdt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gwcptjzmg.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gocjlfzvu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxelaowjg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gqnfbzsdg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gynkejsnh.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gadyanopi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gfomfxofb.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gajvafiih.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gpikcmdgq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gertyspbd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gednggcgo.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gxyyexqrc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gsjylrxhs.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gafhquvir.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gckywfudj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gjbepdixc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/glevfzavd.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gagcliise.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gbbcxcuba.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gddnqesob.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gzyoatdpa.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gkttnwccx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gwvvotfee.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/ggqbilhpy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gbnocffib.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gffmbaohp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gpdgtcdsi.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gzfazkurm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/giszmhkwh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gbdgxamny.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/ggvgovnyd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/geawexlpi.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gxmlahsbs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkyqwvxgc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gsmxagvfo.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/ggdpaeiqi.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gfolebzpu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/grehexpoj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gssvvwtpu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gchhibucs.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gqhshvqnk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gylbirshs.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gexdfynop.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gvxmvqibd.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gxdjfqzhh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxxxsquk.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gcfrnonsi.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gedptcisp.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/glkmluqwn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/grsvpxqqt.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/ggwnscrtp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gdmpcntlz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gyuuyzwld.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/glhoebrao.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/godjrlwxn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gffqwrsns.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxrfghwlc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqpvcmrmc.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gmdwvzafd.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gbpyopvjc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gghqzymdf.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gcgdvnnur.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gebmdvdjm.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gvldfclug.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/ghgvgzjbd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gptzdzvft.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gbpkkjlqc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/glapxoaum.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gukvvqyds.sHtML


<!-- 参考信息 -->