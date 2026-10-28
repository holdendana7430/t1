代发 wailian999

set -euo pipefail
来源：http://hz.feifeiyinyue.top/gtvmufusdd.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtquvmuubo.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gtkguykcjg.html

[R03] 只读变量
来源：http://hz.ehwqpu.com/gtwoygxpwa.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gtxynxxdsj.html

[R04] 位置参数
来源：http://hz.gaohongyu789.top/gtlxzkwjhz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gthixkdxwn.html

[R05] 参数默认值
来源：http://hz.shzxlz.cn/gtslfmuxwl.html

name="${1:-default}"
来源：http://hz.c1oappe.top/gtplekfsmc.html

[R06] 判断命令是否存在
来源：http://hz.xuetiantiany.cn/gtpmcxbdyh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hysaishi.cn/gtelvqxcpf.html

[R07] if 判断文件
来源：http://hz.snrcjt.cn/gtbngsiqle.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.316326.xyz/gthlpuybhw.html

[R08] 数值比较
来源：http://hz.aizwys.cn/gttltqaten.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pengpengdd.cyou/gtifrocrmr.html

[R09] 字符串比较
来源：http://hz.shzxlz.cn/gtzninkpbe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gtapvngugx.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtahvzjbta.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.vqdsnc.cn/gtrkjjpmru.html

[R11] case 多分支
来源：http://hz.daria6918.cn/gtawojvugi.html

case "$1" in
来源：http://hz.hfpthk.cn/gtpizdjqhh.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gthpzfdztz.html

stop)  echo "停止" ;;
来源：http://hz.zhiwuduotai.top/gtffeidmzs.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtcohuplff.html

esac
来源：http://hz.sweek.top/gtvrygrusm.html

[R12] for 遍历文件
来源：http://hz.ydzc1.top/gtzbixojnr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtxcmlxttt.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtgnithrhp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtdvdsacgf.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gtojuhogqt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxuanxn.top/gttoqnyndk.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtwpepqify.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnqzz.top/gtvdrmawnu.html

[R16] until 等待条件
来源：http://hz.guannengcc.top/gtaifsteqa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.iojbl.cn/gtgwwvvbhp.html

[R17] 数组定义与取值
来源：http://hz.dianchejie.cn/gtimazlxub.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gtnkvmyoec.html

[R18] 遍历数组
来源：http://hz.jyoumei.cn/gtscgwslvt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtcmxfydvk.html

[R19] 数组长度
来源：http://hz.zycfv.cn/gtguhjvuzm.html

echo "${#arr[@]}"
来源：http://hz.yvedp.cn/gtjayweuzb.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtsuxjijsy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xingfuxueyuan.xyz/gtjhmifije.html

[R21] 字符串长度
来源：http://hz.xinyue.icu/gtdwoqsruo.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtuwfuhlba.html

[R22] 截取子串
来源：http://hz.xuetiantiany.cn/gteogmljvr.html

echo "${s:0:5}"
来源：http://hz.svipenyu.cn/gtpxsghnuf.html

[R23] 字符串替换
来源：http://hz.shuidangran.top/gtirgemujs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtyetynokb.html

[R24] 大小写转换
来源：http://hz.dianchejie.cn/gtqecckgze.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.birdmap.top/gtagbazhlq.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtzamardwa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.andypj.xyz/gtupdsgqoi.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtdogaakos.html

now=$(date +%F); echo "$now"
来源：http://hz.ybcxt.top/gtsdbzevfw.html

[R27] 算术展开
来源：http://hz.xuanzx.com/gtdmogidqe.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtojjcfnvg.html

[R28] 浮点运算
来源：http://hz.ehwqpu.com/gtfyevbswt.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtbyrtatba.html

[R29] 定义函数
来源：http://hz.cdnleiting.top/gtudzgncbg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.mhx1999.top/gtarqocfye.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gtotifpxxa.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258888.top/gtsiscqwil.html

[R31] 局部变量
来源：http://hz.gotoacloud.top/gtccrnerkw.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtltijsgka.html

[R32] 参数个数校验
来源：http://hz.ywan-chungtsiang.top/gtvrgnjwgd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gzhubu.top/gtvckzcqbs.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtbilxmeyv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gthfcmyjyz.html

[R34] 退出时清理
来源：http://hz.sweek.top/gtrwdbgruy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtkwbiwvlp.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtslocdbmf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtawcyaihd.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtrptnppiw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gteeazlnzy.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtdslfxyqq.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtahqturuf.html

[R38] 管道串联
来源：http://hz.snrcjt.cn/gtyqgcwjgh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shuidangran.top/gttjidhsif.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gtvjskjzor.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtrdbummxr.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtkaudozlt.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtzgnwrkgq.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtqnqzemwk.html

cmd >/dev/null 2>&1
来源：http://hz.dianchejie.cn/gtifhjbyag.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtxgxkjxxr.html

wc -l < a.txt
来源：http://hz.chenjidiqi.icu/gtminpwbzn.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtrbiybdak.html

find . -name "*.log" -type f
来源：http://hz.meibo888.top/gtuyacebpd.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtcbojdcln.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtrypkbqii.html

[R45] 批量删除
来源：http://hz.aibaodan.cn/gthaauxgie.html

find . -name "*.tmp" -delete
来源：http://hz.xingfuxueyuan.xyz/gtvnrjvtjt.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtcfqiqons.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenlongwang.top/gtjihjlymj.html

[R47] sed 单行替换
来源：http://hz.hnxiangtu.top/gtwqvmuejz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtckvsykrt.html

[R48] awk 取指定列
来源：http://hz.xuetiantiany.cn/gtpqjagmnf.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gthwvzyxjl.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gttzyatilf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gzhubu.top/gtmtluklng.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtydlifflf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhengqikj.top/gtptwifzhp.html

[R51] 排序去重取前几
来源：http://hz.xuetiantiany.cn/gtylnwxqjs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtpubccfpv.html

[R52] 统计行数
来源：http://hz.ehwqpu.com/gtutgvackd.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtpvvidkqh.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtjloihhyj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gthvcgvviw.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtnltlafqv.html

diff a.txt b.txt
来源：http://hz.ywan-chungtsiang.top/gtndwgqytk.html

[R55] 压缩与解压
来源：http://hz.yj20258.top/gtzobvxxvr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gtlcbtlkzh.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtkpeankqd.html

scp file user@host:/path/
来源：http://hz.aizwys.cn/gtbxliqthg.html

[R57] 远程执行命令
来源：http://hz.birdmap.top/gtkovaxlmq.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtbzteqzye.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtptpygblg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtrvpnaubn.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gtxzcftovr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sxryk.cn/gtnlxqhapn.html

[R60] 只看 HTTP 状态码
来源：http://hz.c1oappe.top/gtbyllidmu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtntvkmpnr.html

[R61] 磁盘占用
来源：http://hz.mhx1999.top/gtdlgayucp.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtvlrvntzj.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtjxbeubis.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gtqtibuqqm.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gtmzdnleap.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gtdtbweejz.html

[R64] 结束进程
来源：http://hz.yueranfly.top/gtczjrjxek.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtawpmgydo.html

[R65] 查看端口占用
来源：http://hz.yongpay.top/gtnzsvebje.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ppjwa.cn/gtqpavusld.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtqrhbthep.html

crontab -e;  crontab -l
来源：http://hz.haohaochexian.top/gtsxvbqolp.html

[R67] 生成随机十六进制串
来源：http://hz.yuanzhike.top/gtkbwtmvkf.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtrmrzaajb.html

[R68] 计算文件校验值
来源：http://hz.316326.xyz/gtvsrtheer.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jiagoushi.top/gtglhqaawd.html

[R69] 生成随机密码
来源：http://hz.yj20258888.top/gtaesoqmmq.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtwjoijchh.html

[R70] 时间戳与互转
来源：http://hz.daxiang520.top/gtbqakkrht.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gtfzajttqw.html

[R71] 日期格式化
来源：http://hz.svipenyu.cn/gtyozqywnp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhijiandao.cn/gtrdacttnx.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtshysmddi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj202588.top/gtmbrvwclu.html

[R73] 分割大日志
来源：http://hz.nwbrower.top/gtklflaxbp.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtgdhuhbmu.html

[R74] 批量重命名
来源：http://hz.jianghu66.top/gtwecghnqr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cashguo.top/gtuoqccalv.html

[R75] 导出环境变量
来源：http://hz.tanke756.top/gtvmswjbaj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtcrnfflze.html

[R76] 使用临时文件
来源：http://hz.zhoulong.xyz/gtlxyjnzez.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gtlpghuzck.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtcqmeitxo.html

read -rp "请输入: " ans
来源：http://hz.xziqi.cn/gtykrzmbff.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtgzfyltgu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhaomingkeji.xyz/gtzuisbrqf.html

[R79] 解析命令行选项
来源：http://hz.jianghu66.top/gtqjaaiajd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtvzzwfads.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtuiqfywwd.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtrqcobxqu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjeqndvcx.html

S. C / C++ 专题
来源：http://hz.jqgfzy.top/gtvdjueyxy.html

================================================================================
来源：http://hz.nanxuanxn.top/gtieiwityh.html

[S01] C：Hello World
来源：http://hz.9152youxi.cn/gtymqyykbm.html

#include <stdio.h>
来源：http://hz.daria6918.cn/gtrviirofm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jiagoushi.top/gtjdktcekh.html

[S02] C：变量与格式化输出
来源：http://hz.pycfn.com/gtcuwcxqiz.html

int a = 10; printf("%d\n", a);
来源：http://hz.xziqi.cn/gtzistncbf.html

[S03] C：读入整数
来源：http://hz.jqgfzy.top/gtklmfkdfb.html

int x; scanf("%d", &x);
来源：http://hz.sxryk.cn/gteevxjhbx.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtkugbvziy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhaomingkeji.xyz/gtldqlauzu.html

[S05] C：字符串长度
来源：http://hz.sysykeji.top/gtccbfenvy.html

strlen(s)
来源：http://hz.yuxming.cn/gtvtoipyly.html

[S06] C：字符串比较
来源：http://hz.hywenlv.cn/gtljntkoau.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gttmlixmvt.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtvaeqzpnx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtsowcsncq.html

[S08] C：动态内存分配与释放
来源：http://hz.yvedp.cn/gtkgbdtyay.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fengsongda.top/gtzcsnylxi.html

[S09] C：结构体定义与初始化
来源：http://hz.pycfn.com/gtipboqdkv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtojjjigqx.html

[S10] C：指针与解引用
来源：http://hz.c1oappe.top/gtvfsmjddg.html

int *p = &a;  *p = 5;
来源：http://hz.pengpengdd.cyou/gtqicmnhgi.html

[S11] C：逐行读文件
来源：http://hz.c1oappe.top/gtcazihpwb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtuvlislrv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gtnawqvrhn.html

fclose(f);
来源：http://hz.ydjk.org.cn/gtwmvrigvl.html

[S12] C：写文件
来源：http://hz.yonumen.top/gtalayotpb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cashguo.top/gtsadmcabb.html

[S13] C：宏定义
来源：http://hz.zhijiandao.cn/gtouimhewk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cdnleiting.top/gtjydcyave.html

[S14] C：枚举
来源：http://hz.9152youxi.cn/gtqeqxdqud.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgufenzy.top/gtcppvopyd.html

[S15] C：类型转换
来源：http://hz.cdnleiting.top/gtskksviue.html

(double) a / b
来源：http://hz.ybcxt.top/gtbreyjzfi.html

[S16] C：位操作置位
来源：http://hz.xinyue.icu/gthezlkyzi.html

x |= (1 << 3);
来源：http://hz.kuanghao11.cn/gtzislnoke.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtvkynsnli.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtrfhtqdzi.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangtech.top/gtdhekewuu.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtlztvxasz.html

[S19] C：快速排序
来源：http://hz.yueranfly.top/gtbsmvguqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gteogkblld.html

[S20] C：二分查找
来源：http://hz.cucudq.cn/gtueblthnc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtpuubwshw.html

[S21] C：字符类别判断
来源：http://hz.zhoulong.xyz/gtxlkjbyte.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuanzx.com/gtixjjqssd.html

[S22] C：字符串转数字
来源：http://hz.cucudq.cn/gtrzrxdqlo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fzhhl.top/gtlqezhoes.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtrzyiyeik.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.c1oappe.top/gtaknbhdzc.html

[S24] C：获取本地时间
来源：http://hz.jinghuilouyu.cn/gtawhvdedm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtdoggssmr.html

[S25] C：内存拷贝
来源：http://hz.316326.xyz/gtvfktfhsc.html

memcpy(dst, src, n);
来源：http://hz.aibaodan.cn/gtikybzvzw.html

[S26] C：内存清零
来源：http://hz.gzhubu.top/gtpddxsfwj.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtkbnldnrr.html

[S27] C：定义常量
来源：http://hz.zdqjudy.top/gtmcucdgnb.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtvqktyyui.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtsgrxevzy.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gtrhnpsaga.html

[S29] C：变参函数
来源：http://hz.cheryme.top/gtdyehprml.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.feifeiyinyue.top/gtqnwjrvud.html

[S30] C：头文件保护
来源：http://hz.yj20258888.top/gtjcvtnhqw.html

#ifndef X_H
来源：http://hz.quarkkingdee.top/gtdejouihc.html

#define X_H
来源：http://hz.vqdsnc.cn/gtejzbqyzz.html

#endif
来源：http://hz.ywan-chungtsiang.top/gtzlgtdeqq.html

[S31] C++：Hello World
来源：http://hz.cheryme.top/gtmoiqbmrm.html

#include <iostream>
来源：http://hz.hysaishi.cn/gtcwoutoll.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tian-w.cn/gtkbwyuubn.html

[S32] C++：字符串
来源：http://hz.hongshengwenyu.top/gtwnegyapf.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtqpbvqygh.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtejvtngct.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtayrdgkfj.html

[S34] C++：遍历 vector
来源：http://hz.ehwqpu.com/gtvrruorsr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhaomingkeji.xyz/gttsemgmjo.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtcvuittws.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtlmnqlsmv.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtpfkajnzp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtfxrmacez.html

[S37] C++：set
来源：http://hz.smart0.xyz/gtruhiedzd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258.top/gtdqgppfvx.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtmrlnlots.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtyceokkvv.html

[S39] C++：自定义比较器排序
来源：http://hz.quarkkingdee.top/gttxekrbaw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtyakcwadx.html

[S40] C++：查找元素
来源：http://hz.hywenlv.cn/gtmrfhxior.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtoixdsufw.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtdezrnpgk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinghuilouyu.cn/gtxittfhjs.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigfzy.top/gtbrewebqd.html

class B : public Base { public: void f() override {} };
来源：http://hz.gzhubu.top/gtfxxdvmaa.html

[S43] C++：智能指针
来源：http://hz.shzxlz.cn/gtohdeveyt.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gtuqvnqbzx.html

[S44] C++：引用传参
来源：http://hz.hammf.cn/gtvsfimnwz.html

void inc(int &x) { ++x; }
来源：http://hz.hnqzz.top/gtlqdlblrq.html

[S45] C++：lambda
来源：http://hz.yongpay.top/gtbazngrmv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xingfuxueyuan.xyz/gtovylcuyw.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtndkmsrgw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhaomingkeji.xyz/gtcefhnxvl.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtwqalkbdq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sufxvd.cn/gtdquwgpaw.html

[S48] C++：逐行读文件
来源：http://hz.hywenlv.cn/gtmkmwqqtl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dashuyun.cn/gtuuhbxoxj.html

while (std::getline(in, line)) { }
来源：http://hz.sxryk.cn/gttmkrxbko.html

[S49] C++：写文件
来源：http://hz.quarkkingdee.top/gtvpghfltz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xziqi.cn/gtscrvfozk.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtxxwyswmq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.haohaochexian.top/gttzdlkejx.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gtepmaciag.html

static_cast<double>(a) / b
来源：http://hz.tian-w.cn/gtkvzfitvc.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtgyhuevzg.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtuygbdoix.html

[S53] C++：移动语义
来源：http://hz.aizwys.cn/gtwpivcfai.html

std::vector<int> w = std::move(v);
来源：http://hz.zhiwuduotai.top/gtggsanbqx.html

[S54] C++：异常处理
来源：http://hz.tanke756.top/gtrdzhtoxx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xinyue.icu/gtknqcepac.html

[S55] C++：结构化绑定
来源：http://hz.ehwqpu.com/gtujruhlpi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhengqikj.top/gtyrzgsfom.html

[S56] C++：optional
来源：http://hz.c1oappe.top/gtdvpjmdaq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhoulong.xyz/gtspdliklt.html

[S57] C++：编译期常量
来源：http://hz.yvedp.cn/gtddwilkab.html

constexpr int N = 10;
来源：http://hz.gaohongyu789.top/gtdkighfsz.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangkeji.top/gtohyeoypz.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtasfshsfj.html

[S59] C++：静态断言
来源：http://hz.daria6918.cn/gtwuffzwwg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtvdbujwpb.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtkujzldvo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.52xcode.cn/gtayfidtih.html

================================================================================
来源：http://hz.sxryk.cn/gtxhtuavjy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gtuvytfebl.html

================================================================================
来源：http://hz.dashuyun.cn/gtjoombpry.html

[T01] Kotlin：Hello World
来源：http://hz.ydzc1.top/gtanqtczrv.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtzqbmsjda.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gtjspanluy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtlklvjnam.html


<!-- 参考信息 -->