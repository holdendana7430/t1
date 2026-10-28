代发 wailian999

R. Bash 专题
来源：http://hz.gogol.net.cn/gtnymempkp.html

================================================================================
来源：http://hz.fzhhl.top/gtzmtgnwkm.html

[R01] shebang 与严格模式
来源：http://hz.gotoacloud.top/gtycznrbmo.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtywzyhrjd.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtqcptddol.html

[R02] 变量赋值与使用
来源：http://hz.jinqigufen.top/gtovkfabku.html

name="Tom"; echo "$name"
来源：http://hz.xziqi.cn/gtkopnhals.html

[R03] 只读变量
来源：http://hz.gotoacloud.top/gtwbylnmre.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtoieobjpx.html

[R04] 位置参数
来源：http://hz.birdmap.top/gtwohtyeat.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cheryme.top/gtiguxzceo.html

[R05] 参数默认值
来源：http://hz.cdnleiting.top/gtbhtntblw.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtdlsiczok.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtcmjykcwk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtarzxdczk.html

[R07] if 判断文件
来源：http://hz.zdqjudy.top/gtiswpriil.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yonumen.top/gtxdyfjujp.html

[R08] 数值比较
来源：http://hz.gaohongyu789.top/gtbvntkyca.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shangyingyoupin.top/gtsncbndvg.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtuezcfijj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtdtugqojj.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gtrspnrbaq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhoulong.xyz/gtivpzkfnp.html

[R11] case 多分支
来源：http://hz.xuanzx.com/gtxhfwjiat.html

case "$1" in
来源：http://hz.sufxvd.cn/gtrjubdixz.html

start) echo "启动" ;;
来源：http://hz.xziqi.cn/gtmsnfejti.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtjefocwul.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtnjjhydie.html

esac
来源：http://hz.jqgufenzy.top/gtiqecckeb.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtqojtpjcl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgfzy.top/gtcwsibkoh.html

[R13] for 计数循环
来源：http://hz.pycfn.com/gtxdotydys.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cheryme.top/gtnnzcxhvg.html

[R14] C 风格 for
来源：http://hz.meibo888.top/gtwtbkhygp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ybcxt.top/gtlzonrsny.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtftsjnzok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtmkxjzvgw.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtgtxchcac.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sweek.top/gtikxiqpmm.html

[R17] 数组定义与取值
来源：http://hz.zhaomingkeji.xyz/gtqgimvisi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtecmhgqjj.html

[R18] 遍历数组
来源：http://hz.gzhubu.top/gtjpoxcwyf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhijiandao.cn/gtrkrksiyd.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtcclnbovi.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtsxjdubtb.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtnntauoyt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xingfuxueyuan.xyz/gtbnfwdmty.html

[R21] 字符串长度
来源：http://hz.tianlin.xyz/gtsoxcnnqa.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtyofagvki.html

[R22] 截取子串
来源：http://hz.zhoulong.xyz/gticjhwpbi.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtlnhxzxgm.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gtymaqanwh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258.top/gtcxnlhtwo.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtwjkxhowx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gtsmpaskwx.html

[R25] 去后缀 / 去前缀
来源：http://hz.0kj1m.cn/gtagdocwzx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.svipenyu.cn/gtsghhucum.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gtrzphvzpa.html

now=$(date +%F); echo "$now"
来源：http://hz.gzhubu.top/gteshqqaqa.html

[R27] 算术展开
来源：http://hz.nwbrower.top/gtbmhddjjj.html

echo $((1 + 2 * 3))
来源：http://hz.tian-w.cn/gtqbroqxgc.html

[R28] 浮点运算
来源：http://hz.fengsongda.top/gttjlqbdmp.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtdzkfmiua.html

[R29] 定义函数
来源：http://hz.sweek.top/gtlbdmzgbp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgufenzy.top/gtqkfocgka.html

[R30] 函数返回状态码
来源：http://hz.tianlin.xyz/gtutvmszqj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.feifeiyinyue.top/gtohoibjkb.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtxujcdcee.html

f() { local x=1; echo "$x"; }
来源：http://hz.cheryme.top/gtysvzmcyd.html

[R32] 参数个数校验
来源：http://hz.sweek.top/gtzdexmmai.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gthkcahled.html

[R33] 捕获错误并提示行号
来源：http://hz.nwbrower.top/gtcirsrdqc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hnqzz.top/gtgoxaozgr.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtgqompqsc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtfzteiqci.html

[R35] 后台执行并等待
来源：http://hz.dashuyun.cn/gtlxdqqdcc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhiwuduotai.top/gtnfvcrnfy.html

[R36] 并发执行多个任务
来源：http://hz.pengpengdd.cyou/gtgpofxivd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtyhxyhsws.html

[R37] 把输出赋给变量
来源：http://hz.aibaodan.cn/gtymcjmdle.html

files=$(ls -1)
来源：http://hz.yonumen.top/gtidwbiamw.html

[R38] 管道串联
来源：http://hz.birdmap.top/gtzlxzvijk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.svipenyu.cn/gtipsbavru.html

[R39] 重定向标准输出与错误
来源：http://hz.aizwys.cn/gtsbrrjdmh.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtzlgjpunz.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtmqexmsur.html

echo "log" >> out.log
来源：http://hz.xziqi.cn/gtlgpieeod.html

[R41] 丢弃输出
来源：http://hz.kuanghao11.cn/gtjngmwqij.html

cmd >/dev/null 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtcrdshgqw.html

[R42] 输入重定向
来源：http://hz.vqdsnc.cn/gtsjbhssmi.html

wc -l < a.txt
来源：http://hz.yuanzhike.top/gtyxtpzjop.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gtmukkvtnb.html

find . -name "*.log" -type f
来源：http://hz.zhongyouzk.top/gtmwlrgzeh.html

[R44] 按修改时间查找
来源：http://hz.yongpay.top/gtexfhbenm.html

find . -mtime -7 -type f
来源：http://hz.chenlongwang.top/gtzrljbjsm.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gteyzuzndf.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gtwewcxumt.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtackgvrjn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yvedp.cn/gtoylaqvec.html

[R47] sed 单行替换
来源：http://hz.jqgufenzy.top/gtjzoejawy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtijplsfgm.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtpksueeqf.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtcbepeukw.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gtwmrszpml.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gthdymixdl.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtmqwmsugy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtiizdlhfb.html

[R51] 排序去重取前几
来源：http://hz.gogol.net.cn/gtdshtuqbb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxuanxn.top/gtdfxbijbl.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtpmkyandt.html

wc -l a.txt
来源：http://hz.fzhhl.top/gttrowcmhw.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtupkidkmj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gttzvrzdrk.html

[R54] 比较两个文件
来源：http://hz.redwolf501.top/gtzusfalpf.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtzuctbzru.html

[R55] 压缩与解压
来源：http://hz.aibaodan.cn/gtmuuusupk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtieauqjqm.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtrqyuceqi.html

scp file user@host:/path/
来源：http://hz.xinyue.icu/gtpoakawfd.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtzzzujmgn.html

ssh user@host 'uptime'
来源：http://hz.fengsongda.top/gtdsaehzhe.html

[R58] 下载文件
来源：http://hz.gogol.net.cn/gtsufvdfwn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnqzz.top/gtbagqviwh.html

[R59] 发 POST JSON
来源：http://hz.feifeiyinyue.top/gtgdyznwkh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yonumen.top/gtrhdzwwce.html

[R60] 只看 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtakwewlnn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtivajxmwe.html

[R61] 磁盘占用
来源：http://hz.ivvv.top/gtwqmrospe.html

df -h;  du -sh *
来源：http://hz.smart0.xyz/gtmsflohje.html

[R62] 找最占空间的文件
来源：http://hz.jinyuanbaomall.cn/gtbginwsrk.html

du -ah . | sort -rh | head -10
来源：http://hz.c1oappe.top/gtbgmkcqaj.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtlqfocxct.html

free -h;  ps aux | grep nginx
来源：http://hz.0kj1m.cn/gtamxjnikn.html

[R64] 结束进程
来源：http://hz.yvedp.cn/gtkyercdij.html

kill -9 $(pgrep -f app.py)
来源：http://hz.haohaochexian.top/gtldhqolul.html

[R65] 查看端口占用
来源：http://hz.ivvv.top/gtxbmebhqy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cdnleiting.top/gtnzgmilrd.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtcecwmfxg.html

crontab -e;  crontab -l
来源：http://hz.hongshengwenyu.top/gtprmsoeab.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtawmtvsop.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gtsbcwawih.html

[R68] 计算文件校验值
来源：http://hz.yvedp.cn/gttraxgpbp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtnyznlvxt.html

[R69] 生成随机密码
来源：http://hz.kuanghao11.cn/gtaxqwtnjk.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydjk.org.cn/gtyvwkwzjf.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtyjmovczh.html

date +%s;  date -d @1700000000
来源：http://hz.zhongyouzk.top/gtkgidybmf.html

[R71] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gtopepyqyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtewuwlwnw.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtergtzevl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xinyue.icu/gtsrmujukn.html

[R73] 分割大日志
来源：http://hz.ehwqpu.com/gtzedtvzhx.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtxnicftmp.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtngaxmqsp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxuanxn.top/gtlncrjaoe.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gtmogeejto.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yongpay.top/gtwcztvhzj.html

[R76] 使用临时文件
来源：http://hz.dianchejie.cn/gtwiovguys.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtgyxqukei.html

[R77] 读取用户输入
来源：http://hz.gzhubu.top/gtfevtzzbv.html

read -rp "请输入: " ans
来源：http://hz.andypj.xyz/gtxsrqdhpi.html

[R78] 交互式菜单
来源：http://hz.jinghuilouyu.cn/gtgnkhtpyc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gthvudnpfk.html

[R79] 解析命令行选项
来源：http://hz.xuetiantiany.cn/gteowlfoww.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zycfv.cn/gtkowtnipa.html

[R80] 查看脚本执行耗时
来源：http://hz.jiagoushi.top/gthjtjwkpa.html

time ./run.sh
来源：http://hz.9152youxi.cn/gtqtshojxp.html

================================================================================
来源：http://hz.snrcjt.cn/gtynlymkrh.html

S. C / C++ 专题
来源：http://hz.hfpthk.cn/gtiufpjodc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtphehfwsc.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtveqhievd.html

#include <stdio.h>
来源：http://hz.yongpay.top/gthyeiadwn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gthrnjvzmi.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtishlfmlc.html

int a = 10; printf("%d\n", a);
来源：http://hz.snrcjt.cn/gtilaycgsg.html

[S03] C：读入整数
来源：http://hz.hammf.cn/gtfgmrjbyo.html

int x; scanf("%d", &x);
来源：http://hz.jqgufenzy.top/gtmsgyhboy.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtllmmlwml.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtdfzeyqyz.html

[S05] C：字符串长度
来源：http://hz.9152youxi.cn/gtpnzdxjri.html

strlen(s)
来源：http://hz.yanxiufei.cn/gtclvxlwec.html

[S06] C：字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtnuvqqwgq.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtxkrzfavg.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtwnczatzr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hongshengwenyu.top/gtbmisrxaw.html

[S08] C：动态内存分配与释放
来源：http://hz.jiagoushi.top/gtrdpqhuli.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhoulong.xyz/gtltmpbiii.html

[S09] C：结构体定义与初始化
来源：http://hz.yuanzhike.top/gtbziholtl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yvedp.cn/gtkhchgszh.html

[S10] C：指针与解引用
来源：http://hz.aizwys.cn/gtpqisqheb.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtqvhjloml.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtyppvrlqm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gtehgjxdox.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtkjbyubxl.html

fclose(f);
来源：http://hz.smart0.xyz/gtkucehefa.html

[S12] C：写文件
来源：http://hz.aibaodan.cn/gtxcahhhxc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shzxlz.cn/gtywdxwrxy.html

[S13] C：宏定义
来源：http://hz.havefunace.top/gtzseanzbu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtbuusgszz.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtyolvfker.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zdqjudy.top/gtzsmvlrcf.html

[S15] C：类型转换
来源：http://hz.9152youxi.cn/gtwhbrkybm.html

(double) a / b
来源：http://hz.zhongyouzk.top/gttwkoyknw.html

[S16] C：位操作置位
来源：http://hz.yj20258888.top/gtvlrjdzhh.html

x |= (1 << 3);
来源：http://hz.0kj1m.cn/gtbkzxnjkd.html

[S17] C：安全拼接字符串
来源：http://hz.jinghuilouyu.cn/gtfnbejtur.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtmscscmvy.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangtech.top/gtucqgcmzv.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtsylndgqu.html

[S19] C：快速排序
来源：http://hz.xziqi.cn/gtidlaumrd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtshktswle.html

[S20] C：二分查找
来源：http://hz.gaohongyu789.top/gtangeyqpt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gthlydprdq.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangkeji.top/gttsnfvwox.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zdqjudy.top/gtnrkdvhzg.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtgvhtwsdx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenjidiqi.icu/gtqtqqiifp.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtmijiemmy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtzrirtbys.html

[S24] C：获取本地时间
来源：http://hz.daxiang520.top/gtegdjrpdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtydzaawlq.html

[S25] C：内存拷贝
来源：http://hz.wangshuangyany.cn/gtervbutyu.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtlskjemau.html

[S26] C：内存清零
来源：http://hz.jyoumei.cn/gttdbbvfch.html

memset(a, 0, sizeof a);
来源：http://hz.316326.xyz/gtciwdbusl.html

[S27] C：定义常量
来源：http://hz.yuanzhike.top/gtvvrkhjmu.html

const double PI = 3.14159;
来源：http://hz.yonumen.top/gtwklliuge.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtuxermcqg.html

static int counter = 0;
来源：http://hz.xziqi.cn/gtisqwprta.html

[S29] C：变参函数
来源：http://hz.yanxiufei.cn/gtitmnzods.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtbowsqrur.html

[S30] C：头文件保护
来源：http://hz.gzhubu.top/gtnqjxdsyv.html

#ifndef X_H
来源：http://hz.yj202588.top/gtgcvrxgkb.html

#define X_H
来源：http://hz.tian-w.cn/gtwwutwbgz.html

#endif
来源：http://hz.jinqigfzy.top/gtotytslac.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtumumwial.html

#include <iostream>
来源：http://hz.wangdashe.top/gtyhoabfui.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhoulong.xyz/gtbdidkeag.html

[S32] C++：字符串
来源：http://hz.cucudq.cn/gtxjmpjiqi.html

std::string s = "hi";  s += "!";
来源：http://hz.hywenlv.cn/gtazyikhwl.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtbiclxxdb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgufenzy.top/gtymeeenqp.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gtosepbunj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hywenlv.cn/gtdavhzsbk.html

[S35] C++：map
来源：http://hz.meibo888.top/gtrajjywgz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtapoyyolt.html

[S36] C++：unordered_map
来源：http://hz.cqqwz.cn/gtuyjvxfjn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtmqlalgeg.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtkshrmuri.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtyevgirzb.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtvabmwlhx.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gtxxgzjvrw.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtulfaexhw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtidmhqngh.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gtnusccwvl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fzhhl.top/gtrwsohvso.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangtech.top/gtopkttxyi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gtozwdlhbd.html

[S42] C++：继承与虚函数
来源：http://hz.feifeiyinyue.top/gtpuqyrskm.html

class B : public Base { public: void f() override {} };
来源：http://hz.dashuyun.cn/gtxxoaznew.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtbazwzjkl.html

auto p = std::make_unique<int>(5);
来源：http://hz.fengsongda.top/gtqyrixscm.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtxxfsgett.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtqdpehsct.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtjvpnczfo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtaujcqkdn.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gthkmjzhdm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhaomingkeji.xyz/gthlfjpmdy.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuxming.cn/gtreaxacle.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daxiang520.top/gtwvffabcc.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtwkjmfydy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ybcxt.top/gtusbbrypv.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gtgsuqbnmj.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtvlpfbykp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtbmvcedxp.html

[S50] C++：格式化数字
来源：http://hz.feifeiyinyue.top/gtayeryekh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtweucunyz.html

[S51] C++：显式类型转换
来源：http://hz.shuidangran.top/gtlwlkxptu.html

static_cast<double>(a) / b
来源：http://hz.gogol.net.cn/gtuvcvvdes.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtidihfheg.html

int size() const noexcept { return n_; }
来源：http://hz.tian-w.cn/gttgxfkmul.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtkxzqmzmb.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtoqwneued.html

[S54] C++：异常处理
来源：http://hz.fzhhl.top/gtvezpuqkk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtqyzngycg.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gtsgmmzhyb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangdashe.top/gtqbccrdjb.html

[S56] C++：optional
来源：http://hz.aizwys.cn/gtxpkodhfe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhengqikj.top/gtpjufvwew.html

[S57] C++：编译期常量
来源：http://hz.gaohongyu789.top/gtaoemmyga.html

constexpr int N = 10;
来源：http://hz.havefunace.top/gtsnkibozs.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtcqwykxfr.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj202588.top/gtfkfpkdme.html

[S59] C++：静态断言
来源：http://hz.zycfv.cn/gtnnkxvdcg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtstvvihbf.html

[S60] C++：遍历并删除元素
来源：http://hz.cucudq.cn/gtxuoedlnu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jyoumei.cn/gteymadxun.html

================================================================================
来源：http://hz.shuidangran.top/gtzidwnbuw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtflsibkpx.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtbdykjpda.html


<!-- 参考信息 -->