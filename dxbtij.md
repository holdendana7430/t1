代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gtzxacnaor.html

[Q90] 生成序号列
来源：http://hz.ppjwa.cn/gtsmgwdubo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.316326.xyz/gtygdicrku.html

================================================================================
来源：http://hz.svipenyu.cn/gtubcycxvz.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtyswmmhkw.html

================================================================================
来源：http://hz.nanxinkj.top/gtcpuuedax.html

[R01] shebang 与严格模式
来源：http://hz.sweek.top/gtodpalarq.html

#!/usr/bin/env bash
来源：http://hz.jqgufenzy.top/gtvhwfbaxu.html

set -euo pipefail
来源：http://hz.zhoulong.xyz/gtzeabvblj.html

[R02] 变量赋值与使用
来源：http://hz.yj202588.top/gthiqkfqhd.html

name="Tom"; echo "$name"
来源：http://hz.cashguo.top/gtpxiqofmv.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gtkzlvnejd.html

readonly PI=3.14
来源：http://hz.andypj.xyz/gtqykzvxyf.html

[R04] 位置参数
来源：http://hz.yonumen.top/gtdlzqzlcb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gtcrizxbqz.html

[R05] 参数默认值
来源：http://hz.zhaomingkeji.xyz/gtccvcccaw.html

name="${1:-default}"
来源：http://hz.yj20258.top/gtodtbpged.html

[R06] 判断命令是否存在
来源：http://hz.meibo888.top/gtgwitwmnx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ppjwa.cn/gtzxcxqcrv.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gtnzzznlfd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangshuangyany.cn/gtknlpsxif.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtpgcxvyxg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtmbkkqkuu.html

[R09] 字符串比较
来源：http://hz.yvedp.cn/gtrvcmslpy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dashuyun.cn/gtzhgapqza.html

[R10] 正则匹配
来源：http://hz.hysaishi.cn/gtybwdcfid.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtybbavvmw.html

[R11] case 多分支
来源：http://hz.fengsongda.top/gtucgdkbkq.html

case "$1" in
来源：http://hz.hnqzz.top/gtqcnaprct.html

start) echo "启动" ;;
来源：http://hz.yueranfly.top/gtzcxzhnmo.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtdxacoxci.html

*)     echo "未知命令" ;;
来源：http://hz.cqqwz.cn/gtplbsmclj.html

esac
来源：http://hz.pycfn.com/gtulfltybl.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtuingpjsq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sufxvd.cn/gtycgygywm.html

[R13] for 计数循环
来源：http://hz.xuetiantiany.cn/gtwzoomadu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shzxlz.cn/gtpildhqix.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtijgnsbuz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtepodwkbj.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gtgelatybe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jianghu66.top/gtszkjzmxz.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtpyfhnisp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tianlin.xyz/gtyhdisgmi.html

[R17] 数组定义与取值
来源：http://hz.daxiang520.top/gtlrzkjcir.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daxiang520.top/gtufsvlccn.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtitookuwy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shangyingyoupin.top/gtsgphufdx.html

[R19] 数组长度
来源：http://hz.zhixingplan.top/gtvgdgfvbp.html

echo "${#arr[@]}"
来源：http://hz.cashguo.top/gtoqnzcort.html

[R20] 关联数组（字典）
来源：http://hz.9152youxi.cn/gthtjesbco.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtefwcxuuk.html

[R21] 字符串长度
来源：http://hz.zhoulong.xyz/gtmwoldkes.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtpuotfbsw.html

[R22] 截取子串
来源：http://hz.jlsjyb.cn/gtiiccsaqt.html

echo "${s:0:5}"
来源：http://hz.chenzaomai.com/gtucnuhskj.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtysxpnauo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhongyouzk.top/gtulmitozb.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gttdmfrnyy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtyhzbjbfi.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtfzajtxij.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shzxlz.cn/gtxuilnjbg.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gtkjjsyqzr.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258.top/gtbivxbzxj.html

[R27] 算术展开
来源：http://hz.chenzaomai.com/gtkgsavzos.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gtdvjvoucw.html

[R28] 浮点运算
来源：http://hz.shangyingyoupin.top/gthwmrazjm.html

echo "scale=2; 10/3" | bc
来源：http://hz.daxiang520.top/gtgxwbaerx.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gtlqusasuz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnqzz.top/gtrgiaekbo.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtamqtdmvk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtmpszalrc.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtgnxnivrr.html

f() { local x=1; echo "$x"; }
来源：http://hz.haohaochexian.top/gthacfuqzu.html

[R32] 参数个数校验
来源：http://hz.zhiwuduotai.top/gtlmvlyqhy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtrxconzti.html

[R33] 捕获错误并提示行号
来源：http://hz.havefunace.top/gtgobmonyp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258.top/gtqafzhwbp.html

[R34] 退出时清理
来源：http://hz.chenzaomai.com/gtkrgfakhx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtlzgymhcz.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtdiimokfy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtxlwqpnkt.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtpfxiibrv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aizwys.cn/gtycsetvui.html

[R37] 把输出赋给变量
来源：http://hz.chenzaomai.com/gtqqtgvciz.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtgjyvzyhp.html

[R38] 管道串联
来源：http://hz.chenjidiqi.icu/gtzjlsyytr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydjk.org.cn/gtzqlvrlsn.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtawkystdm.html

cmd > out.log 2>&1
来源：http://hz.9152youxi.cn/gtkdsrkjjc.html

[R40] 追加写日志
来源：http://hz.ydjk.org.cn/gtfssfqrro.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtvuibxqko.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtubevyldl.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtcrfhcyvp.html

[R42] 输入重定向
来源：http://hz.xziqi.cn/gtlqvppejp.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtdnzfcdln.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtfntifgcm.html

find . -name "*.log" -type f
来源：http://hz.chenjidiqi.icu/gtbosfsqbe.html

[R44] 按修改时间查找
来源：http://hz.pengpengdd.cyou/gtegupxezf.html

find . -mtime -7 -type f
来源：http://hz.tianlin.xyz/gtbqemlmvm.html

[R45] 批量删除
来源：http://hz.smart0.xyz/gtzkebbvdr.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gteoaonona.html

[R46] 递归替换文件内容
来源：http://hz.jqgufenzy.top/gtsfsfazrm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtosiethoa.html

[R47] sed 单行替换
来源：http://hz.ehwqpu.com/gtnlyrrldh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenlongwang.top/gtsnbjfhzn.html

[R48] awk 取指定列
来源：http://hz.sweek.top/gtkgvvfmsr.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtuydxmoge.html

[R49] awk 带条件
来源：http://hz.nanxinkj.top/gtenrensxk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gtrrngxlxm.html

[R50] awk 求和
来源：http://hz.vqdsnc.cn/gtvurqekze.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtejmkwmep.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gtauukviit.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gttfyighef.html

[R52] 统计行数
来源：http://hz.yonumen.top/gtlcjeezgv.html

wc -l a.txt
来源：http://hz.kuanghao11.cn/gtxiwwvvuy.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtnsbkyxpv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.c1oappe.top/gtakdsntnn.html

[R54] 比较两个文件
来源：http://hz.ehwqpu.com/gtgnoieair.html

diff a.txt b.txt
来源：http://hz.jinghuilouyu.cn/gtbrhrwidt.html

[R55] 压缩与解压
来源：http://hz.pengpengdd.cyou/gtuvtwaoxo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtsnumwuya.html

[R56] 远程拷贝
来源：http://hz.sxryk.cn/gtjuntytvv.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gtnmnjqtpy.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtqvykhmov.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtfohllqyu.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtvojxkbki.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yongpay.top/gtdthncyek.html

[R59] 发 POST JSON
来源：http://hz.yj20258888.top/gtphiavfen.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigufen.top/gtfazewcuv.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhixingplan.top/gtufuwcagt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtowzunzvo.html

[R61] 磁盘占用
来源：http://hz.xuetiantiany.cn/gtukxvlwmv.html

df -h;  du -sh *
来源：http://hz.sufxvd.cn/gtmzjrmdse.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtefflbntg.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtfgwtweev.html

[R63] 内存与进程
来源：http://hz.jinqigfzy.top/gtoharaxqc.html

free -h;  ps aux | grep nginx
来源：http://hz.fzhhl.top/gtbdzfqmet.html

[R64] 结束进程
来源：http://hz.chenlongwang.top/gtzxflrrfi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gttcrjxaei.html

[R65] 查看端口占用
来源：http://hz.iojbl.cn/gtcialzwpn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtmqxziswk.html

[R66] 定时任务
来源：http://hz.redwolf501.top/gtzwxhhkuw.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtzywtrcfu.html

[R67] 生成随机十六进制串
来源：http://hz.gotoacloud.top/gtqvwywuhn.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtjcnqpgak.html

[R68] 计算文件校验值
来源：http://hz.hnxiangtu.top/gtbsriqooo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jiagoushi.top/gtldherpjk.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gtlfoqsmcn.html

head -c 16 /dev/urandom | base64
来源：http://hz.9152youxi.cn/gtqqszunnz.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtfhrowcwe.html

date +%s;  date -d @1700000000
来源：http://hz.gotoacloud.top/gtcqmbsnbg.html

[R71] 日期格式化
来源：http://hz.iojbl.cn/gtpzotmrxo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgufenzy.top/gtnlsfkoui.html

[R72] 等待端口就绪
来源：http://hz.zhijiandao.cn/gtwshnqkpb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guannengcc.top/gtjjkygahj.html

[R73] 分割大日志
来源：http://hz.hfpthk.cn/gtdnkkwkks.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtgeyilywn.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gtksaiqvll.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtrbkszsay.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gtadueelyl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtnehuznaj.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gthicprjef.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtqzxxhqfv.html

[R77] 读取用户输入
来源：http://hz.gotoacloud.top/gtlvqqowqv.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gtdvhhoxgr.html

[R78] 交互式菜单
来源：http://hz.guowangkeji.top/gtjxvkxbjt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hongshengwenyu.top/gtbxgzxeqj.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtqauszfbp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cqqwz.cn/gtrhxbiytm.html

[R80] 查看脚本执行耗时
来源：http://hz.quarkkingdee.top/gtuumwoqup.html

time ./run.sh
来源：http://hz.smart0.xyz/gtslmynubb.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpgyfzywb.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtzjasgcxx.html

================================================================================
来源：http://hz.jinqigufen.top/gtpfdkjmsh.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtoxibofac.html

#include <stdio.h>
来源：http://hz.jqgfzy.top/gtlrsyjaov.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.snrcjt.cn/gtusiftggg.html

[S02] C：变量与格式化输出
来源：http://hz.yuanzhike.top/gtjgpshxom.html

int a = 10; printf("%d\n", a);
来源：http://hz.ywan-chungtsiang.top/gtdxlorura.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtmvyepbew.html

int x; scanf("%d", &x);
来源：http://hz.xuanzx.com/gtjlrsklzv.html

[S04] C：字符串复制
来源：http://hz.jlsjyb.cn/gtrlcgeocv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gogol.net.cn/gtxumvlcjv.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtcascwkmw.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtrcieiizu.html

[S06] C：字符串比较
来源：http://hz.fzhhl.top/gthddagqjn.html

strcmp(a, b) == 0
来源：http://hz.ydzc1.top/gtoogpxgjj.html

[S07] C：数组遍历求和
来源：http://hz.ybcxt.top/gtrryfxxex.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtnfjempeo.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtbarirgpm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtneiyemee.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtslvejhmk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.svipenyu.cn/gtvkbenalx.html

[S10] C：指针与解引用
来源：http://hz.c1oappe.top/gtejijitpd.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtwrshznjm.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtvqzabrop.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtlhpvcrtm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangdashe.top/gtrlulldbf.html

fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtcdggdkse.html

[S12] C：写文件
来源：http://hz.guowangkeji.top/gtwaixoghq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtvlywdgij.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gtrbstuzdn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shangyingyoupin.top/gtqjtntrkf.html

[S14] C：枚举
来源：http://hz.yangfankeji.com/gtffallmtr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtqqekwhsf.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtphukfidg.html

(double) a / b
来源：http://hz.yueranfly.top/gtwweponhb.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtqmsxnnsl.html

x |= (1 << 3);
来源：http://hz.cashguo.top/gtkzlngfwi.html

[S17] C：安全拼接字符串
来源：http://hz.wangdashe.top/gtvpvjneah.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xingfuxueyuan.xyz/gtmnsetkda.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtskqljzyn.html

int main(int argc, char **argv)
来源：http://hz.9152youxi.cn/gtaeoimsma.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gtjnujfqwa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtezxpharb.html

[S20] C：二分查找
来源：http://hz.fzhhl.top/gtilbukwfg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtsmxakdtg.html

[S21] C：字符类别判断
来源：http://hz.smart0.xyz/gtaduffbwg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangshuangyany.cn/gtvibpxwvm.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtrrldmzin.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtarxqjzli.html

[S23] C：随机数
来源：http://hz.hongshengwenyu.top/gtgzshxoki.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.9152youxi.cn/gtmvzdfrdq.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtkyugejhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuetiantiany.cn/gtoxtfmhph.html

[S25] C：内存拷贝
来源：http://hz.xingfuxueyuan.xyz/gtvgimdhrh.html

memcpy(dst, src, n);
来源：http://hz.yuxming.cn/gtievyxlbr.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gthglmizoi.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtjehyxdqm.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtnlkhxlja.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtxyflygug.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtbrzuiwwn.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtzvmpjrta.html

[S29] C：变参函数
来源：http://hz.zhiwuduotai.top/gtigdnbypf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinyuanbaomall.cn/gtfmkzxfqz.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtmsfnpjzc.html

#ifndef X_H
来源：http://hz.birdmap.top/gtzsisfmxj.html

#define X_H
来源：http://hz.xylfe.cn/gtmueyocrj.html

#endif
来源：http://hz.zhongyouzk.top/gtcfxctxvx.html

[S31] C++：Hello World
来源：http://hz.jlsjyb.cn/gtknwxpbxp.html

#include <iostream>
来源：http://hz.birdmap.top/gtlvfxtutn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.havefunace.top/gtgxblwjsb.html

[S32] C++：字符串
来源：http://hz.yongpay.top/gthmlkmgwj.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtjxwjorwz.html

[S33] C++：vector 增删
来源：http://hz.fzhhl.top/gtqdvfvpmq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtfvmtbzys.html

[S34] C++：遍历 vector
来源：http://hz.pengpengdd.cyou/gtgspnhyhc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.iojbl.cn/gtjsmvdzcs.html

[S35] C++：map
来源：http://hz.sweek.top/gtmcotypel.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtuvcktrni.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtwdamwpnv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtqtvztsmx.html

[S37] C++：set
来源：http://hz.meibo888.top/gthvacswco.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtnjdcnprp.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtsrgumafp.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtpjvfsmlf.html

[S39] C++：自定义比较器排序
来源：http://hz.aizwys.cn/gtpwrbhmuo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aizwys.cn/gtqyfobbms.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtvnrvkncn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258.top/gtsvofyixn.html

[S41] C++：类与构造函数
来源：http://hz.xziqi.cn/gttvujwlsd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fzhhl.top/gtbbjbiihu.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gtbcmxzrok.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenjidiqi.icu/gtloqsjbns.html

[S43] C++：智能指针
来源：http://hz.hywenlv.cn/gtjgzwppsz.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gtcihptouq.html

[S44] C++：引用传参
来源：http://hz.meibo888.top/gtfrguuinw.html

void inc(int &x) { ++x; }
来源：http://hz.yj202588.top/gtpbwumfqw.html

[S45] C++：lambda
来源：http://hz.hammf.cn/gtgwyhulgr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtsvbmnctg.html

[S46] C++：函数模板
来源：http://hz.hysaishi.cn/gtncxjebit.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.birdmap.top/gturckccme.html

[S47] C++：结构化绑定遍历
来源：http://hz.gotoacloud.top/gtrxroaamr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtdvfjtdxx.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtxulsmmpu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtaxgjowab.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtpinfejow.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtiguphwdo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fzhhl.top/gtelkzqfzm.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtschvytwi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhoulong.xyz/gtoivhbaei.html

[S51] C++：显式类型转换
来源：http://hz.cdnleiting.top/gtijvifdvf.html

static_cast<double>(a) / b
来源：http://hz.nanxuanxn.top/gtytmvdayv.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtmlioeguq.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gthjsrmqog.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gthdmlfsig.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangkeji.top/gtetapkhfr.html

[S54] C++：异常处理
来源：http://hz.0kj1m.cn/gtekcjlvun.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtigznuniq.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtugxhkgbg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinyuanbaomall.cn/gtyeshpnsx.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtwhijybiz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.snrcjt.cn/gtrdevklhz.html

[S57] C++：编译期常量
来源：http://hz.gzhubu.top/gtgymoqxrj.html

constexpr int N = 10;
来源：http://hz.yonumen.top/gtihqdzplx.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtqhnkwpdq.html

namespace ns { int f() { return 1; } }
来源：http://hz.feifeiyinyue.top/gteukixnrr.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtblzhklmi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtkottvboa.html

[S60] C++：遍历并删除元素
来源：http://hz.jiagoushi.top/gtmiwucaxm.html


<!-- 参考信息 -->