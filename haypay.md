代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtwfhiwlrx.html

[Q90] 生成序号列
来源：http://hz.ppjwa.cn/gtuylmgeyo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtmtaqyisk.html

================================================================================
来源：http://hz.jiagoushi.top/gtklqbljrs.html

R. Bash 专题
来源：http://hz.jinqigfzy.top/gtjusdvkod.html

================================================================================
来源：http://hz.pycfn.com/gtkmoduvpr.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtvppnxyrz.html

#!/usr/bin/env bash
来源：http://hz.sxryk.cn/gtocjdcjne.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gtbcncpjaz.html

[R02] 变量赋值与使用
来源：http://hz.fzhhl.top/gtepfgicbq.html

name="Tom"; echo "$name"
来源：http://hz.zhijiandao.cn/gtxmttffql.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gtrenclhep.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtttichngl.html

[R04] 位置参数
来源：http://hz.sufxvd.cn/gthjjnuuoi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtcammpbbr.html

[R05] 参数默认值
来源：http://hz.hywenlv.cn/gtxsajqzdl.html

name="${1:-default}"
来源：http://hz.dianchejie.cn/gtozbaoqki.html

[R06] 判断命令是否存在
来源：http://hz.aizwys.cn/gtdwycykrc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtlfxxtula.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtnioxeojy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhixingplan.top/gtfhrtymgg.html

[R08] 数值比较
来源：http://hz.bjfxy.top/gtmzjbndnm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pengpengdd.cyou/gtdchqaqyg.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gtmzqzxnvy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guowangkeji.top/gtxlxnghml.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtiedeevws.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.mhx1999.top/gtzxsyptst.html

[R11] case 多分支
来源：http://hz.316326.xyz/gthgclxeai.html

case "$1" in
来源：http://hz.sweek.top/gtuxfvpliu.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtpntxmamb.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtudoxsuli.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gtsxqvhgnp.html

esac
来源：http://hz.hammf.cn/gtsnafowlk.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gthbmnwtym.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhongyouzk.top/gtdbctytwz.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtdzzvcqep.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtjsraiern.html

[R14] C 风格 for
来源：http://hz.fzhhl.top/gtmpvwhovy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtzgispenj.html

[R15] while 逐行读文件
来源：http://hz.gogol.net.cn/gtykzlfque.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.havefunace.top/gtvobmqfxx.html

[R16] until 等待条件
来源：http://hz.zycfv.cn/gtbzprroqj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gtzixwainu.html

[R17] 数组定义与取值
来源：http://hz.hfpthk.cn/gtciqijkma.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtrlhmuiqd.html

[R18] 遍历数组
来源：http://hz.52xcode.cn/gtkberbgjv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.vqdsnc.cn/gtpafxnjra.html

[R19] 数组长度
来源：http://hz.sysykeji.top/gtcewugijr.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtvjtzfxas.html

[R20] 关联数组（字典）
来源：http://hz.c1oappe.top/gtrhgwcooo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pycfn.com/gtqppvlihq.html

[R21] 字符串长度
来源：http://hz.hysaishi.cn/gthnzntytq.html

echo "${#s}"
来源：http://hz.wangdashe.top/gtkfiieynl.html

[R22] 截取子串
来源：http://hz.zycfv.cn/gtecqyeich.html

echo "${s:0:5}"
来源：http://hz.zhijiandao.cn/gtohtjxjrd.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gthvaevzmu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.andypj.xyz/gttkwrubph.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtadgxamcv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guannengcc.top/gtacfueuds.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtlthixytn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgufenzy.top/gtoqvpuhmh.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtcktivcdy.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtsfvkznyj.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtpybabevk.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtxasldfhb.html

[R28] 浮点运算
来源：http://hz.ybcxt.top/gtmgfddabi.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnqzz.top/gtswiqxpoo.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtqfiykrij.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtndmffezf.html

[R30] 函数返回状态码
来源：http://hz.tian-w.cn/gtgjcnghfv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gtxitfxpew.html

[R31] 局部变量
来源：http://hz.9152youxi.cn/gtffmcduee.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtulhlojng.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtwtcteapv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.meibo888.top/gtrnrdihqt.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtweozwrau.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtilqixjlp.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtiuourtkh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtnfccblku.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtaamxtuug.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinghuilouyu.cn/gtgpoihhcf.html

[R36] 并发执行多个任务
来源：http://hz.gogol.net.cn/gtwcnhwtwl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fzhhl.top/gtjfquloes.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gtekworgzr.html

files=$(ls -1)
来源：http://hz.yonumen.top/gttgsashtv.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gtqejfvhxm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtqcidiurv.html

[R39] 重定向标准输出与错误
来源：http://hz.tanke756.top/gtdhrrbzpp.html

cmd > out.log 2>&1
来源：http://hz.hysaishi.cn/gtpudekcjf.html

[R40] 追加写日志
来源：http://hz.zhengqikj.top/gtpqunbsff.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtxifkblkx.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtwdcsxzcs.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtikikwryh.html

[R42] 输入重定向
来源：http://hz.tanke756.top/gtbilnnabj.html

wc -l < a.txt
来源：http://hz.nwbrower.top/gtqickoinh.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtlxbhrzfe.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtzvdtlczz.html

[R44] 按修改时间查找
来源：http://hz.vqdsnc.cn/gtghzjyvnt.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gteywuppxj.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gttclwrcbf.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigufen.top/gtqgejpcod.html

[R46] 递归替换文件内容
来源：http://hz.redwolf501.top/gtxcellnbq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xylfe.cn/gterdoijkt.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gtypttcmly.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtoaysibve.html

[R48] awk 取指定列
来源：http://hz.shangyingyoupin.top/gtlxzgrjns.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangshuangyany.cn/gtyteuswoj.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtfdkqmahq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dashuyun.cn/gtofpjllxw.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtsnkrwnea.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenlongwang.top/gtfapaxgza.html

[R51] 排序去重取前几
来源：http://hz.ywan-chungtsiang.top/gtzjeswwdw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aizwys.cn/gtiuppalwp.html

[R52] 统计行数
来源：http://hz.wangshuangyany.cn/gtbyqihmcd.html

wc -l a.txt
来源：http://hz.chenzaomai.com/gteiwupeob.html

[R53] 查看文件头与实时尾
来源：http://hz.xylfe.cn/gtpspecuxp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daxiang520.top/gtyxawwiax.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtubpycftr.html

diff a.txt b.txt
来源：http://hz.havefunace.top/gtcuhcrxxh.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gttyabkscq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gtygtrqqjj.html

[R56] 远程拷贝
来源：http://hz.xziqi.cn/gtljhnlzhi.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtcjfrlwtd.html

[R57] 远程执行命令
来源：http://hz.ydjk.org.cn/gthvtmsvac.html

ssh user@host 'uptime'
来源：http://hz.ivvv.top/gtqpyqkuos.html

[R58] 下载文件
来源：http://hz.wangshuangyany.cn/gthmeazvpc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gtoidnlkiw.html

[R59] 发 POST JSON
来源：http://hz.hammf.cn/gtwskmwovw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhiwuduotai.top/gtmkkbwmsh.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigufen.top/gthzfbdnwj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guannengcc.top/gtjsyvfvzt.html

[R61] 磁盘占用
来源：http://hz.zycfv.cn/gtkarlaoyl.html

df -h;  du -sh *
来源：http://hz.guowangkeji.top/gttjuwaszy.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gtxjnxjhcl.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gtrgsbxuvz.html

[R63] 内存与进程
来源：http://hz.ybcxt.top/gtffuctoxa.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtwayzzrfz.html

[R64] 结束进程
来源：http://hz.dashuyun.cn/gtineghkdd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtxcxghvaj.html

[R65] 查看端口占用
来源：http://hz.nanxuanxn.top/gtpgdboawr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.pengpengdd.cyou/gtkreagwox.html

[R66] 定时任务
来源：http://hz.shangyingyoupin.top/gtrsvjvmop.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtmbfbzkgk.html

[R67] 生成随机十六进制串
来源：http://hz.haohaochexian.top/gtsxjdliap.html

openssl rand -hex 16
来源：http://hz.cashguo.top/gtuggiykxv.html

[R68] 计算文件校验值
来源：http://hz.nanxuanxn.top/gtvtppgupg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xylfe.cn/gthfxtqhdh.html

[R69] 生成随机密码
来源：http://hz.havefunace.top/gthzzimuto.html

head -c 16 /dev/urandom | base64
来源：http://hz.cqqwz.cn/gtmulkdklu.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtcmamruia.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtzcmxesjp.html

[R71] 日期格式化
来源：http://hz.iojbl.cn/gttazlegoq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtilwfekza.html

[R72] 等待端口就绪
来源：http://hz.hywenlv.cn/gtzndvfcqb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtuajjhnqo.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtifqumlxh.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtbcldaeje.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gtwaefpmqy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aizwys.cn/gtgovmcxfy.html

[R75] 导出环境变量
来源：http://hz.shangyingyoupin.top/gtvjjpvkai.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtbwfzzafb.html

[R76] 使用临时文件
来源：http://hz.hammf.cn/gtxvuzhmct.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtxeghuhto.html

[R77] 读取用户输入
来源：http://hz.havefunace.top/gtfvbuhngq.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtxddrjjbo.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtdhcuvlqq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtzwfqtuto.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtcvosckub.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gtmiqgnfpf.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gttfkcuhzg.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtxpkqlnbv.html

================================================================================
来源：http://hz.zhengqikj.top/gtchtnuoms.html

S. C / C++ 专题
来源：http://hz.wangshuangyany.cn/gtacfqqvgg.html

================================================================================
来源：http://hz.ppjwa.cn/gthmfcohou.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gtawdixmuj.html

#include <stdio.h>
来源：http://hz.daria6918.cn/gtftezkbxu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtwxsmqsxm.html

[S02] C：变量与格式化输出
来源：http://hz.hnxiangtu.top/gtybrtnxvq.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258.top/gtlrfguqbr.html

[S03] C：读入整数
来源：http://hz.sxryk.cn/gtghjzeuou.html

int x; scanf("%d", &x);
来源：http://hz.shangyingyoupin.top/gtidbdtizk.html

[S04] C：字符串复制
来源：http://hz.mhx1999.top/gtxqixotny.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhengqikj.top/gtbvvdslcl.html

[S05] C：字符串长度
来源：http://hz.vqdsnc.cn/gtjhumcgmp.html

strlen(s)
来源：http://hz.daxiang520.top/gtwbrqaewa.html

[S06] C：字符串比较
来源：http://hz.chenlongwang.top/gtpxpsordc.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtohpquwma.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtduvtmxiu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gtmtmwojtr.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtpdagjojv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtxjkqjkch.html

[S09] C：结构体定义与初始化
来源：http://hz.daxiang520.top/gtgfactbkh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sysykeji.top/gtfrdydnps.html

[S10] C：指针与解引用
来源：http://hz.ydzc1.top/gtpvcmyctr.html

int *p = &a;  *p = 5;
来源：http://hz.chenzaomai.com/gtfzbfrdcu.html

[S11] C：逐行读文件
来源：http://hz.9152youxi.cn/gtmiipufcl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtqmnmbasl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pengpengdd.cyou/gtnldzqbqq.html

fclose(f);
来源：http://hz.hammf.cn/gthrygvter.html

[S12] C：写文件
来源：http://hz.birdmap.top/gtywtrfdik.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtomxusvdx.html

[S13] C：宏定义
来源：http://hz.chenzaomai.com/gtnjpuxbqb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aizwys.cn/gtagytitfp.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtuarvykyk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guannengcc.top/gtgccuyuur.html

[S15] C：类型转换
来源：http://hz.nwbrower.top/gtmeigcaly.html

(double) a / b
来源：http://hz.yuxming.cn/gtkxfekqdm.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gtajhvhkgq.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtbfvpvsmg.html

[S17] C：安全拼接字符串
来源：http://hz.zhengqikj.top/gtcytyegcy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydjk.org.cn/gtukwfvcmq.html

[S18] C：命令行参数
来源：http://hz.gzhubu.top/gtpodvtoks.html

int main(int argc, char **argv)
来源：http://hz.cdnleiting.top/gtwkahfcti.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtmqjmfzgh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtucgerrjg.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gtlyjzdgss.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtkdyvqmic.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtgohsvqao.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangdashe.top/gtmpfshaip.html

[S22] C：字符串转数字
来源：http://hz.xylfe.cn/gtlnkyttqk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenlongwang.top/gtgovretif.html

[S23] C：随机数
来源：http://hz.shzxlz.cn/gtrfjjmsao.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gteiwkncbn.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gthmxmylyk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.9152youxi.cn/gtsmpylybv.html

[S25] C：内存拷贝
来源：http://hz.aibaodan.cn/gtohjmefxo.html

memcpy(dst, src, n);
来源：http://hz.zhengqikj.top/gtmhvmcbpw.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtqgxyizrn.html

memset(a, 0, sizeof a);
来源：http://hz.316326.xyz/gtohqvwles.html

[S27] C：定义常量
来源：http://hz.hfpthk.cn/gtgvnietzh.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gthcgduzps.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtlfbqsshg.html

static int counter = 0;
来源：http://hz.redwolf501.top/gtajbszmic.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtxeaokygq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gtftjoycbf.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtqsqorhab.html

#ifndef X_H
来源：http://hz.sweek.top/gtmtmvbzsw.html

#define X_H
来源：http://hz.shanyushiyangkeji.top/gtgpfynoyz.html

#endif
来源：http://hz.sufxvd.cn/gtnwcinczu.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtofhnkwsw.html

#include <iostream>
来源：http://hz.yongpay.top/gteoerttba.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guannengcc.top/gtvlmltydz.html

[S32] C++：字符串
来源：http://hz.zhengqikj.top/gtakumtaux.html

std::string s = "hi";  s += "!";
来源：http://hz.zhaomingkeji.xyz/gtgskvfvap.html

[S33] C++：vector 增删
来源：http://hz.yongpay.top/gtoyrvvetq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtrlqztfuv.html

[S34] C++：遍历 vector
来源：http://hz.chenzaomai.com/gtfieovdtm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hywenlv.cn/gtuqarfzyq.html

[S35] C++：map
来源：http://hz.yangfankeji.com/gtkzhxjswk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtaueolexb.html

[S36] C++：unordered_map
来源：http://hz.yvedp.cn/gtohlohinj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtnolggvcv.html

[S37] C++：set
来源：http://hz.fzhhl.top/gtpakxkuzi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.9152youxi.cn/gtythaqdii.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gtmojyfivi.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtavmrxmmn.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258.top/gtvmsvgfln.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtjgswrnwm.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtxikrpvzs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.9152youxi.cn/gtksiwmreh.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtbsvnynfe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtxaafkeoy.html

[S42] C++：继承与虚函数
来源：http://hz.birdmap.top/gtzaujovsp.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtshbfmbhr.html

[S43] C++：智能指针
来源：http://hz.cashguo.top/gtiaubozfj.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtkorqaope.html

[S44] C++：引用传参
来源：http://hz.kuanghao11.cn/gtzgxhpmtw.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtoynldiqo.html

[S45] C++：lambda
来源：http://hz.chenzaomai.com/gtbynkmrmh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtnurrfqmo.html

[S46] C++：函数模板
来源：http://hz.feifeiyinyue.top/gtzezbysru.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pycfn.com/gtkvymeaha.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtfxqkizci.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.smart0.xyz/gttucmzqkd.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gthirjltaw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aizwys.cn/gtfzveyixd.html

while (std::getline(in, line)) { }
来源：http://hz.zhongyouzk.top/gtduyouesu.html

[S49] C++：写文件
来源：http://hz.pengpengdd.cyou/gthyszbaia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtbutddmxe.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangkeji.top/gtguxasnew.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtpoggalxn.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gtufhazoyo.html

static_cast<double>(a) / b
来源：http://hz.smart0.xyz/gtuukmszyh.html

[S52] C++：const 与 noexcept
来源：http://hz.9152youxi.cn/gttfqowzqu.html

int size() const noexcept { return n_; }
来源：http://hz.zhoulong.xyz/gtldqcshxj.html

[S53] C++：移动语义
来源：http://hz.zhixingplan.top/gtiuscydeo.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigufen.top/gtdjwanxan.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtkjqhtkfz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangtech.top/gtlnhxsxez.html

[S55] C++：结构化绑定
来源：http://hz.ydjk.org.cn/gtzstaoyqt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gtzslkzjln.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gtjkfhrkqz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daxiang520.top/gtzpcburst.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gthqghwxio.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gttegyixgy.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gtmesgmsug.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuxming.cn/gthttzwacs.html

[S59] C++：静态断言
来源：http://hz.jyoumei.cn/gtznovibxa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhijiandao.cn/gtwdkcsbqq.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtordclzhb.html


<!-- 参考信息 -->