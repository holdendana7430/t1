代发 wailian999

esac
来源：http://www.share.fehbvm.com/Article/details/gjkgbsqvt.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gcmqkbsez.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/grswttcru.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/geprqlgxk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtxwoxcjk.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gaxiftixp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gtsykkcur.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/guzyahdzk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gkzxkaurt.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gbduzeako.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gbqqrcwrp.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gbvkgpwqm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gzkgeticw.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gumddkbpo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gyxuvomvg.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/goymurnxo.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gwrrhzfci.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gfishdkse.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/giylptqhm.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gqzgxnlgk.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gdyvqsimk.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/ghpmpysrm.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gjelaucrq.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gwvgpaidw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gytqhltrn.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gngrsrpey.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gbbgstiny.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gbekkodqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gnlifwmge.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gzccprpjk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gdawfplti.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gfwpzwgnm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gcqcfnerf.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gzfonhnuj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gkmymvujz.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gjoigoykt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gmqhztfrc.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gfraeffwc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gvnakzpyg.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gjeyaivfc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/geeghybxw.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gwdehodiw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkcbbnzk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gcukoqqgj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/ggloamthw.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gqljznnpv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gvqhyaede.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gibunjryz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gjoupsjjf.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gidcalade.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gwrnstufy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gnvodyadp.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/glfadlwih.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gbmwcqrsf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gbptaqmho.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gpjibeoud.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gdrtoqnbc.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/grglxlkgv.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gnjbuqcdp.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/ggbntesep.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjtynqogb.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gpktnrjeb.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gwaolfoua.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/geaxvqpza.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gfxesidnp.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gybuklatt.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gkwkczxoq.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/ghgdicuvv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gpojqohvz.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gqqfhhkfc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/glcxnjesu.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gmldtiboq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gmgkacpcj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gwisojtdc.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/ghrbjzxgw.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gkebqnrqo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gcjnvtgqj.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gztangtkt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gnkhdhmjx.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gwiblipgc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gihvnkxzd.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/ghwmjrlug.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gxyqpryxz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gwttvahzg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gcqlpccxw.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gdqucimql.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/ghjrfckrb.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gclnaiqbq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/grjmasafr.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gsarxrqmm.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gkwwmctnl.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gphqzrmey.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gaahdadhy.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gwqfddsks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gcmcoylmi.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gwqazcpyu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/geqfpwaoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gkficyqie.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gpaofebww.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gjsjkpnpq.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/geeshqxuc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/glqeowzpi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gnygedcry.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gqxyysxqg.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/goedntces.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/goloznwyo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gyaxzzenp.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gypuspkid.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gjjippqpb.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/ghykltmdb.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gwlmcmaga.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gwacvcpmt.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gudjvwwkn.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gcpcxbkka.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gpzaqhtyh.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gmzdzljvg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/guntmhwjj.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gitpwmkdp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gjvpvbqic.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gbuaeuupb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gthrlkzul.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gqkspvzeu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gmomtlukz.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/goptrkqds.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gqwtkyquj.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gwsirtzfm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gclcdbxxp.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gedgmbkvc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/ghehahbuy.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gqafiaydw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gmosxeyhh.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/grhqpltoz.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gypuyrdwz.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gjqdltvfh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/ggqlprguf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/ghgrikfqv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggojenkgp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gehvqnvwk.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gvqckmhuw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggqselckq.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gdfxgnpvm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwtqirajn.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzpaztmny.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gjdmanpfz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gvzvikcmz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/govintufp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gykokouxb.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gaxwasldz.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gceohrtjf.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gvrzgresq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gwwrubdbv.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/grncsvvxp.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gpfgptwmg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gkdbeddhc.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gjcqgwhje.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gzbhwkxqs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gzhmmdfha.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gqtegnoee.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gxgfqvpak.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gpbrjvome.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/glydcimfr.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/geobzpeop.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gscbjdsfn.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gvzifsgro.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gauqxzcwt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gakunhonl.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/grzoxetdr.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gfpwfxqpm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gyiagprlm.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gfrxpvkij.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gtqskbyqd.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gyhazkfqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/ggdrsvtef.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gwanhwvms.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gucfnkpey.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gxujflnlv.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gvbaeysxg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwxdyavpj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/ghcccwait.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/glvrsxqhh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gouvsinpu.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gcuxztylw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gphsmjisu.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gqjqdktcv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghncrzgdj.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/girmmphgs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gxtxmrnnd.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gqrlsgrqk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gdkgeynmi.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gteirzbix.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gcwvgpnia.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gvokurmgg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gotsblahg.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gkpaeeaep.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gqqivlfdd.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gndaxitxk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gjvdxfmvm.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gidihvomk.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gndjlbcfo.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gcsmxmtoc.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gdkqacxyc.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/guypefdnl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gidezpzlj.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gfxznzgld.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/ghzwrpkov.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/ghhmxsqsh.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gpruhfjrl.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gojxcvlnq.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gwglyanpd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gblfprrcp.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gagvkothl.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gmoghitya.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gbwyhpady.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gtyetwbtb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gqfevsbuo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/grxyckwnz.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gadatjpuy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkpgrgstk.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gxzdpdsyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gnvtmhkrp.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gjpeusvbj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghcpqevfp.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gtufxkjpx.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gchkwwoif.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gbtqaxvdl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gsdjhpfwf.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gruwxzwyj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gqyremqis.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/guxzidhqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gyinjyjmy.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gljwohunl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gjcdecksz.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gyscirzfm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/ghgnnpjxq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/glljjmwgv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrgoehor.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gbahseerg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gsxfxewbl.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gaqgwmyrl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gaofogusf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gnwekgjvp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gvncryvaj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gksmfapqp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gcegopmnt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gzdtftgpr.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gtutrhkzp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gcklhpatn.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gxminerch.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/goqteawqh.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gtjswcshb.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/ggxkuagmo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gybyfzalu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gvmttdpds.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gmjpwbawm.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gbencyznk.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/guyweespx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gmufiaxfs.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gsgcpgciv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gshlkkdvb.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gskvdpqdn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gfmegqxok.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/genkznrgk.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gwuwrpzir.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ghrpmyqyc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gwgbczsyb.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/grwctbncd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ggtsxgaut.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/grrlbudta.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gipbyjwyv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpgioakor.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gxqvosune.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnxitdbdj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtcbtotcr.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gceruzpnd.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gnczojlcz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gpblqodjd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gvzyxmmqg.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gteebymqk.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gimnbvarj.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gmzyrdxuk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gagyvddka.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gutdjccqz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gyyhujrpj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gvigvnzcx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gbmjpcpqj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gbuwfcrqp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gywilabkd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ghavbomjv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gokxvjbyj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gzhsawzsn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/guttbwyld.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gkjrtvwul.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gbqesqiko.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gqyblfbgl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gbjpbbgev.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzcrtbuvr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gdjzoffrn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvtpbzit.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gsrhxjqgd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gyhdiwkzd.sHtML


<!-- 参考信息 -->