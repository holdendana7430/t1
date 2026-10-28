代发 wailian999

R. Bash 专题
来源：http://hz.52xcode.cn/gtxlwpblcg.html

================================================================================
来源：http://hz.zdqjudy.top/gtglgbnysy.html

[R01] shebang 与严格模式
来源：http://hz.havefunace.top/gtjtexioiu.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gthfejlzps.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtsddrcfhm.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtxkbuqetq.html

name="Tom"; echo "$name"
来源：http://hz.vqdsnc.cn/gttgebpccj.html

[R03] 只读变量
来源：http://hz.sysykeji.top/gtczjsrsqd.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtlkaixsos.html

[R04] 位置参数
来源：http://hz.gaohongyu789.top/gtiesqnods.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.bjfxy.top/gtqcjtnqnl.html

[R05] 参数默认值
来源：http://hz.tanke756.top/gtcgrjownj.html

name="${1:-default}"
来源：http://hz.xuanzx.com/gtekzvnvsr.html

[R06] 判断命令是否存在
来源：http://hz.jqgufenzy.top/gtrmewaqpk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xylfe.cn/gtjgwgjjgn.html

[R07] if 判断文件
来源：http://hz.yj20258888.top/gtztzjdmlg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangkeji.top/gtzxjegxkf.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gthvlzkbzp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtkemixbiv.html

[R09] 字符串比较
来源：http://hz.yongpay.top/gtyvgfoabg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258.top/gtkpgfpnix.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtcfzwygno.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtwmjzxytz.html

[R11] case 多分支
来源：http://hz.nanxinkj.top/gtgwmsiaxk.html

case "$1" in
来源：http://hz.zycfv.cn/gtryrzsrje.html

start) echo "启动" ;;
来源：http://hz.kuanghao11.cn/gtviefeyii.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtwyrsvbgg.html

*)     echo "未知命令" ;;
来源：http://hz.svipenyu.cn/gtmdsypuxe.html

esac
来源：http://hz.jiagoushi.top/gttpbtumqq.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtnmoqlhrt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shangyingyoupin.top/gtyyjwaoyq.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtvhcfcufv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtpdgiumyg.html

[R14] C 风格 for
来源：http://hz.xylfe.cn/gtngxggido.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yueranfly.top/gtgjttuvvn.html

[R15] while 逐行读文件
来源：http://hz.52xcode.cn/gtfhlmmwtc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtpulecvwk.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtcvqgdytj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xziqi.cn/gtteuqvcwo.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtfuqiuipl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gttujbgpbq.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtmratxwvo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xziqi.cn/gtfadpfjpw.html

[R19] 数组长度
来源：http://hz.jinghuilouyu.cn/gtazsgpfkq.html

echo "${#arr[@]}"
来源：http://hz.chenjidiqi.icu/gtdewcxjun.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtjddwxcmz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhongyouzk.top/gtlcruuvch.html

[R21] 字符串长度
来源：http://hz.chenjidiqi.icu/gtwihichhs.html

echo "${#s}"
来源：http://hz.wangdashe.top/gtplcmqkdh.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtbbxxyiic.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gtogprhfyf.html

[R23] 字符串替换
来源：http://hz.redwolf501.top/gtcmfzgvkk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gtquttywpu.html

[R24] 大小写转换
来源：http://hz.yvedp.cn/gtwnjwydda.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yangfankeji.com/gtvampbqwk.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtfrrggfkk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gtbmndkndy.html

[R26] 命令替换
来源：http://hz.shangyingyoupin.top/gtvihipsxj.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gthtbnwuzl.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtzgvzdbvx.html

echo $((1 + 2 * 3))
来源：http://hz.ehwqpu.com/gtpzvozazn.html

[R28] 浮点运算
来源：http://hz.chenjidiqi.icu/gtipgsogkp.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhongyouzk.top/gtmsjqxzkt.html

[R29] 定义函数
来源：http://hz.yangfankeji.com/gtghtrthmw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ehwqpu.com/gtndqncpgk.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtejrradzg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtqbytsdbc.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtudlyafou.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtvwhpicko.html

[R32] 参数个数校验
来源：http://hz.ppjwa.cn/gtelgkryty.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gtuuqzelvc.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtbhedlrvb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtzdswemdj.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtsgilwtum.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtfuivhghf.html

[R35] 后台执行并等待
来源：http://hz.iojbl.cn/gtatfgdwbv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sysykeji.top/gtdutvxnvk.html

[R36] 并发执行多个任务
来源：http://hz.chenlongwang.top/gtfajkjqcc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hfpthk.cn/gttdgrxaac.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtgyhpyldh.html

files=$(ls -1)
来源：http://hz.yangfankeji.com/gtixmrxmei.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtvlpdcgve.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yvedp.cn/gtngcpnzyo.html

[R39] 重定向标准输出与错误
来源：http://hz.gaohongyu789.top/gtfiapgoct.html

cmd > out.log 2>&1
来源：http://hz.tanke756.top/gtxopbryhb.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtqwgxmibg.html

echo "log" >> out.log
来源：http://hz.guannengcc.top/gtddylxwdn.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtdzixhbtu.html

cmd >/dev/null 2>&1
来源：http://hz.fzhhl.top/gtmmftglrw.html

[R42] 输入重定向
来源：http://hz.shangyingyoupin.top/gtyfgjuuhc.html

wc -l < a.txt
来源：http://hz.chenzaomai.com/gtbisryjbm.html

[R43] 按名字查找文件
来源：http://hz.xuetiantiany.cn/gtwieasday.html

find . -name "*.log" -type f
来源：http://hz.yuxming.cn/gtmkldlruu.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtxxyudmuw.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtibigvrlq.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gthpmmkegr.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtpmyvlwjd.html

[R46] 递归替换文件内容
来源：http://hz.vqdsnc.cn/gtzzmsjcjx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.svipenyu.cn/gtwqqlynjw.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtptlccouo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gtgmjveidr.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtweapyldt.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtvohftmjg.html

[R49] awk 带条件
来源：http://hz.mhx1999.top/gtdatlsica.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cashguo.top/gtchxyysbs.html

[R50] awk 求和
来源：http://hz.jianghu66.top/gtzpptnpii.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtekxsqgyx.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtfbsxltgs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.iojbl.cn/gtdlqszupm.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gtyovnrdng.html

wc -l a.txt
来源：http://hz.cashguo.top/gtdhwezlqg.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtwxlffrdv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtgurpfkwe.html

[R54] 比较两个文件
来源：http://hz.andypj.xyz/gtojixtqnl.html

diff a.txt b.txt
来源：http://hz.dashuyun.cn/gtxtrdskhn.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtxwqusqln.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtqijarbnb.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtxfhgbxim.html

scp file user@host:/path/
来源：http://hz.guannengcc.top/gtqzwwvwcg.html

[R57] 远程执行命令
来源：http://hz.0kj1m.cn/gtqajusjez.html

ssh user@host 'uptime'
来源：http://hz.nanxuanxn.top/gtanhdbhwa.html

[R58] 下载文件
来源：http://hz.gotoacloud.top/gtjkzvchhw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtboneqfbs.html

[R59] 发 POST JSON
来源：http://hz.gaohongyu789.top/gtudsmgjsb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhoulong.xyz/gtmbojhmjg.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtvxvhmmzz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtvyjmdluc.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtukdtkasw.html

df -h;  du -sh *
来源：http://hz.sufxvd.cn/gtwsguiuyv.html

[R62] 找最占空间的文件
来源：http://hz.cucudq.cn/gtufapfzwk.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtabsedljx.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtqloxdldn.html

free -h;  ps aux | grep nginx
来源：http://hz.zycfv.cn/gtzdcjusdu.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gtcaurjfns.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtddjmkltv.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gthrrejpvz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fzhhl.top/gtbbjozikj.html

[R66] 定时任务
来源：http://hz.yj20258.top/gtyoubngvv.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gthwtuuurn.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gtprkiinhh.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gtduimfgyb.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gtjxbtqzhq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnxiangtu.top/gthynmacwi.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtekgecwbr.html

head -c 16 /dev/urandom | base64
来源：http://hz.feifeiyinyue.top/gtvwdoklsl.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gthdcvzdyi.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gtsmcwllci.html

[R71] 日期格式化
来源：http://hz.xinyue.icu/gtxskbrflt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yvedp.cn/gtkrxqnrfs.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtmzsbllvu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuanzhike.top/gtbvqateve.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtegrtnbzs.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtarujfagt.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gtizwgwrue.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangkeji.top/gtocsiecga.html

[R75] 导出环境变量
来源：http://hz.shangyingyoupin.top/gtfxwblyjg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.9152youxi.cn/gtjztowxue.html

[R76] 使用临时文件
来源：http://hz.jqgufenzy.top/gtqsmefnle.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtnpokjtma.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtqphivnqr.html

read -rp "请输入: " ans
来源：http://hz.zhiwuduotai.top/gtyeluwtau.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtixjwnskf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ehwqpu.com/gtdykhwwiu.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gtesnzcuhq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtnxacvdsa.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gtzxgrlbya.html

time ./run.sh
来源：http://hz.bjfxy.top/gtoxvkffnr.html

================================================================================
来源：http://hz.52xcode.cn/gtkrnapfhu.html

S. C / C++ 专题
来源：http://hz.jiagoushi.top/gtwmgytjuq.html

================================================================================
来源：http://hz.hnqzz.top/gtvglmrcgn.html

[S01] C：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtheqnsnsl.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtfzpbmajl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cashguo.top/gtolbicsym.html

[S02] C：变量与格式化输出
来源：http://hz.birdmap.top/gtsjgceicb.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gtjqayhqaf.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtjevcivxs.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtpehxkiab.html

[S04] C：字符串复制
来源：http://hz.jinqigfzy.top/gtuafzrohv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yonumen.top/gtiweaghtf.html

[S05] C：字符串长度
来源：http://hz.jqgfzy.top/gtqjluwori.html

strlen(s)
来源：http://hz.hywenlv.cn/gtgpbnhwgj.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtpstdzhkg.html

strcmp(a, b) == 0
来源：http://hz.nanxinkj.top/gtgjupnnrh.html

[S07] C：数组遍历求和
来源：http://hz.ydzc1.top/gtetoosqgg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxuanxn.top/gtfxxspamv.html

[S08] C：动态内存分配与释放
来源：http://hz.jianghu66.top/gtwxkylcwb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgfzy.top/gtnzyedpuk.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gthmkwtssu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258.top/gtaqixhuta.html

[S10] C：指针与解引用
来源：http://hz.zhixingplan.top/gtnfmhaois.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtwrnskimy.html

[S11] C：逐行读文件
来源：http://hz.tanke756.top/gtwicodqlm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtsvnnseoq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.meibo888.top/gtyabrxnjt.html

fclose(f);
来源：http://hz.cashguo.top/gthsbfcrsp.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtztxylmia.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtesjhoefh.html

[S13] C：宏定义
来源：http://hz.xziqi.cn/gtvituidzq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtllfqcuwc.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtqbeansxm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtbgrraldf.html

[S15] C：类型转换
来源：http://hz.ivvv.top/gtybshroac.html

(double) a / b
来源：http://hz.yangfankeji.com/gtfiennmul.html

[S16] C：位操作置位
来源：http://hz.hysaishi.cn/gtmaetsiqg.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtjeoxcrlg.html

[S17] C：安全拼接字符串
来源：http://hz.jianghu66.top/gtruowqzkm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtccqrhufr.html

[S18] C：命令行参数
来源：http://hz.jqgufenzy.top/gtbwtzseia.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gtsmikrgkp.html

[S19] C：快速排序
来源：http://hz.shangyingyoupin.top/gtnrfylokx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtqgexjqap.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gtwnldatmr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtqvwswwmc.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtxxnwejwg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hnxiangtu.top/gtiwmejfuy.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtrsycpuit.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtiugvwjzh.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtjnyqchpq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtgakcnpvo.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtohpwtayi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtdolgrzam.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtuevlvkcb.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtmzpdzren.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtylencxva.html

memset(a, 0, sizeof a);
来源：http://hz.hfpthk.cn/gtqwdousmp.html

[S27] C：定义常量
来源：http://hz.zhixingplan.top/gtvnktmgst.html

const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtxaisthoy.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gtydoifykh.html

static int counter = 0;
来源：http://hz.yongpay.top/gtzhcpvghi.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtsrkercdu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtbzhqfvlf.html

[S30] C：头文件保护
来源：http://hz.c1oappe.top/gtpijzuaph.html

#ifndef X_H
来源：http://hz.9152youxi.cn/gttbpqdzsv.html

#define X_H
来源：http://hz.tian-w.cn/gtmqwxvdat.html

#endif
来源：http://hz.yonumen.top/gtvmpamlkm.html

[S31] C++：Hello World
来源：http://hz.jiagoushi.top/gtpxnjnhty.html

#include <iostream>
来源：http://hz.fzhhl.top/gthhpmkevz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuanzhike.top/gtxnqtxewa.html

[S32] C++：字符串
来源：http://hz.daxiang520.top/gtcthmtlmp.html

std::string s = "hi";  s += "!";
来源：http://hz.gzhubu.top/gtibyxmeof.html

[S33] C++：vector 增删
来源：http://hz.zhongyouzk.top/gtxzqfyqfb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuanzhike.top/gtxoooysps.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gtcjhlcqan.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtqqwpxyag.html

[S35] C++：map
来源：http://hz.feifeiyinyue.top/gtcxpaqccz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtbqxhnamk.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtklehdbhz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtfqxuoeox.html

[S37] C++：set
来源：http://hz.xingfuxueyuan.xyz/gtecjgydvj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtacmywhtk.html

[S38] C++：排序
来源：http://hz.zhiwuduotai.top/gtkhjewufw.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtpgbudobg.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtaobanrjp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.quarkkingdee.top/gtjnexsmhr.html

[S40] C++：查找元素
来源：http://hz.gotoacloud.top/gthmkyhbxy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydzc1.top/gtzevcvmjf.html

[S41] C++：类与构造函数
来源：http://hz.guannengcc.top/gtgrgkvhbz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gttsiosazw.html

[S42] C++：继承与虚函数
来源：http://hz.yvedp.cn/gtqsvwvtct.html

class B : public Base { public: void f() override {} };
来源：http://hz.gzhubu.top/gtegwdwygb.html

[S43] C++：智能指针
来源：http://hz.mhx1999.top/gtyiyuwvxj.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj202588.top/gtyfeqhwin.html

[S44] C++：引用传参
来源：http://hz.sufxvd.cn/gtrbscfgue.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtcwrusibr.html

[S45] C++：lambda
来源：http://hz.jinqigfzy.top/gtgbsmevie.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtvqsnwpeo.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gtzddjvvla.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtbabbevya.html

[S47] C++：结构化绑定遍历
来源：http://hz.yongpay.top/gthbcrtjeq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtbaiwbfpl.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtdatnmxgo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtwmiqxyah.html

while (std::getline(in, line)) { }
来源：http://hz.aizwys.cn/gtgxllvhpg.html

[S49] C++：写文件
来源：http://hz.xylfe.cn/gtrcedgdpy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhoulong.xyz/gtzxhaucvl.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtyhffxhng.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtpxmqyrlw.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtjouapnsr.html

static_cast<double>(a) / b
来源：http://hz.nanxuanxn.top/gtbowgvpbk.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gtpuweqysc.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtobrfmpaw.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtivpfwwqd.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtwcemzhgs.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gthgzgiuso.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daria6918.cn/gtzeltwyor.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtfvgdgiuq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.bjfxy.top/gtfplflscc.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtmkwwaszx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hysaishi.cn/gtstqsggbl.html

[S57] C++：编译期常量
来源：http://hz.birdmap.top/gtnsdhucte.html

constexpr int N = 10;
来源：http://hz.wangshuangyany.cn/gtqohbhgoa.html

[S58] C++：命名空间
来源：http://hz.feifeiyinyue.top/gtrtgumxsm.html

namespace ns { int f() { return 1; } }
来源：http://hz.havefunace.top/gtsixawygc.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtxepqsemb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shzxlz.cn/gtjpybhjod.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtemwatlof.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtjwikbdlg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtakzkgfxf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gtqesgqzvo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmdxucqfm.html


<!-- 参考信息 -->