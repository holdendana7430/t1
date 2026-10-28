代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.redwolf501.top/gttyqfyiwc.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gthoielyjc.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gthiiygseh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.redwolf501.top/gtzdvjbenf.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtgatryowa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinyuanbaomall.cn/gtikoeaypg.html

[Q87] JSON 字段做条件
来源：http://hz.mhx1999.top/gtpfkxgozy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gthwyraubt.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gtgyjnjtje.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtkyovahoc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.havefunace.top/gtzclxuipe.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtkmhnllly.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ivvv.top/gtwnguadmw.html

[Q90] 生成序号列
来源：http://hz.vqdsnc.cn/gtginutpmt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sysykeji.top/gtyybokksg.html

================================================================================
来源：http://hz.jianghu66.top/gtunbduvwx.html

R. Bash 专题
来源：http://hz.svipenyu.cn/gteuqigsgg.html

================================================================================
来源：http://hz.redwolf501.top/gtyjojcouo.html

[R01] shebang 与严格模式
来源：http://hz.cqqwz.cn/gtmiqbgpjh.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtaykshjxl.html

set -euo pipefail
来源：http://hz.nanxuanxn.top/gtibugygps.html

[R02] 变量赋值与使用
来源：http://hz.hammf.cn/gtjfshebrc.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtkzkuuhop.html

[R03] 只读变量
来源：http://hz.yueranfly.top/gtglffmhtu.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtbsaieaes.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gtbnnbxhpu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gtovrwtqbx.html

[R05] 参数默认值
来源：http://hz.tianlin.xyz/gticpcyseh.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtgjadlzfc.html

[R06] 判断命令是否存在
来源：http://hz.hammf.cn/gtpureufqd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gogol.net.cn/gtttpezmtd.html

[R07] if 判断文件
来源：http://hz.snrcjt.cn/gtcpztagvj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtnervjrpv.html

[R08] 数值比较
来源：http://hz.0kj1m.cn/gtmctlvimx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shangyingyoupin.top/gtfbfzrtba.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtibkgdwrl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aibaodan.cn/gtvzlddmxf.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtltznpjql.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtizjtftnm.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gtfvhmdwyr.html

case "$1" in
来源：http://hz.jqgfzy.top/gtxaguoccv.html

start) echo "启动" ;;
来源：http://hz.sysykeji.top/gttomgcova.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtnhbolqgu.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gtddysmnpf.html

esac
来源：http://hz.shzxlz.cn/gtvqhdlrrr.html

[R12] for 遍历文件
来源：http://hz.shangyingyoupin.top/gtcufdmhwn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtcvxlhiha.html

[R13] for 计数循环
来源：http://hz.haohaochexian.top/gtaqdrhqpz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtnuaqxnuu.html

[R14] C 风格 for
来源：http://hz.xylfe.cn/gttnmmgkme.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gtzsftxudx.html

[R15] while 逐行读文件
来源：http://hz.ppjwa.cn/gtdqiiuxuf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gteiuuoupu.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtoxxdwbeb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtpmsvthpq.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtbvevgqbi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhixingplan.top/gtktitqkot.html

[R18] 遍历数组
来源：http://hz.cqqwz.cn/gtjevczgux.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtotsyckhm.html

[R19] 数组长度
来源：http://hz.dianchejie.cn/gtpupbfcyw.html

echo "${#arr[@]}"
来源：http://hz.yanxiufei.cn/gtcpydcukp.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtuosdbzyb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydjk.org.cn/gtvhaqzapd.html

[R21] 字符串长度
来源：http://hz.birdmap.top/gtdbueirbi.html

echo "${#s}"
来源：http://hz.tian-w.cn/gtcpvpoovu.html

[R22] 截取子串
来源：http://hz.dianchejie.cn/gtwwkgtntx.html

echo "${s:0:5}"
来源：http://hz.bjfxy.top/gtfabeefei.html

[R23] 字符串替换
来源：http://hz.vqdsnc.cn/gtapxjbpzz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haohaochexian.top/gttbsqvurl.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtsekpvpfj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dashuyun.cn/gtyhkqshiv.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gttouuwwab.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtktcfiyba.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gtkidakjds.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gttbaymfqr.html

[R27] 算术展开
来源：http://hz.jyoumei.cn/gtduxrrcop.html

echo $((1 + 2 * 3))
来源：http://hz.hywenlv.cn/gttmjjgumb.html

[R28] 浮点运算
来源：http://hz.ybcxt.top/gtoyyhuxqd.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhoulong.xyz/gtmskzaerd.html

[R29] 定义函数
来源：http://hz.fzhhl.top/gtjzexrxpc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shuidangran.top/gtjkmurtwb.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtebfslcrl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.smart0.xyz/gtczfvqnvu.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtjmlqlxhd.html

f() { local x=1; echo "$x"; }
来源：http://hz.9152youxi.cn/gtgdueyosb.html

[R32] 参数个数校验
来源：http://hz.sweek.top/gtdxzdlrkj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.redwolf501.top/gtjyqujhqc.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gtzlonqjlg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gtjeheglhx.html

[R34] 退出时清理
来源：http://hz.c1oappe.top/gtaukrhqyd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sysykeji.top/gtrtdsausz.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtcomvczzl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtdaovpiuq.html

[R36] 并发执行多个任务
来源：http://hz.yvedp.cn/gtjejyarvy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtirdvtxtx.html

[R37] 把输出赋给变量
来源：http://hz.ywan-chungtsiang.top/gtnvghlkur.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtxhlnnhff.html

[R38] 管道串联
来源：http://hz.zhijiandao.cn/gtygdcuqcd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtvjxyepyz.html

[R39] 重定向标准输出与错误
来源：http://hz.jiagoushi.top/gtqlwkecds.html

cmd > out.log 2>&1
来源：http://hz.cashguo.top/gtdnixwcyq.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gthvtjeuid.html

echo "log" >> out.log
来源：http://hz.fzhhl.top/gtiiqjhkia.html

[R41] 丢弃输出
来源：http://hz.dashuyun.cn/gtrekmwyut.html

cmd >/dev/null 2>&1
来源：http://hz.jinyuanbaomall.cn/gtkbnvbqwg.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtdwrlgoto.html

wc -l < a.txt
来源：http://hz.jinyuanbaomall.cn/gtsphfigin.html

[R43] 按名字查找文件
来源：http://hz.nanxuanxn.top/gtwdmgbwyp.html

find . -name "*.log" -type f
来源：http://hz.tian-w.cn/gtiajgyyuk.html

[R44] 按修改时间查找
来源：http://hz.xuanzx.com/gtralqvnlc.html

find . -mtime -7 -type f
来源：http://hz.zycfv.cn/gtcbifeelw.html

[R45] 批量删除
来源：http://hz.jinghuilouyu.cn/gtfegrqirr.html

find . -name "*.tmp" -delete
来源：http://hz.gotoacloud.top/gtzkzizpbh.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtdvggebto.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhijiandao.cn/gtbkswgoim.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gtjrxlgcxg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtqhlznynk.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtrfebtuwz.html

awk '{print $1, $3}' a.txt
来源：http://hz.ppjwa.cn/gtnmecmbtg.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtkizjednc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtknpsozbt.html

[R50] awk 求和
来源：http://hz.meibo888.top/gtoegpmwzk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sweek.top/gtasbgjtuj.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtljycftlh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangtech.top/gtemfjcjci.html

[R52] 统计行数
来源：http://hz.gotoacloud.top/gtgvsmiubd.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtzffkgkmb.html

[R53] 查看文件头与实时尾
来源：http://hz.c1oappe.top/gtrynzhtpo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gtgpbdrocz.html

[R54] 比较两个文件
来源：http://hz.zhoulong.xyz/gtyyjemslc.html

diff a.txt b.txt
来源：http://hz.shanyushiyangtech.top/gtybhihmcb.html

[R55] 压缩与解压
来源：http://hz.hnqzz.top/gtazwvovvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gtjdlrzaol.html

[R56] 远程拷贝
来源：http://hz.zhoulong.xyz/gtkwwjuopl.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtgrctdgfm.html

[R57] 远程执行命令
来源：http://hz.gotoacloud.top/gthenzwzde.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtisbcblvy.html

[R58] 下载文件
来源：http://hz.smart0.xyz/gtxpfkdvfo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gtnaagwxgy.html

[R59] 发 POST JSON
来源：http://hz.316326.xyz/gtlkmhygmb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtdsjduipl.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtbqckksba.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cqqwz.cn/gtjrzqueev.html

[R61] 磁盘占用
来源：http://hz.ehwqpu.com/gtvsszxenj.html

df -h;  du -sh *
来源：http://hz.dashuyun.cn/gtpcvaabuh.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtwkluptlu.html

du -ah . | sort -rh | head -10
来源：http://hz.mhx1999.top/gtvqggzemy.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtktyklmhe.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gteghkhsnm.html

[R64] 结束进程
来源：http://hz.ydjk.org.cn/gthnuhucgj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pycfn.com/gtvewrlnil.html

[R65] 查看端口占用
来源：http://hz.gzhubu.top/gtnkwzdcwg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangkeji.top/gtnvjeuclp.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gtunxyihwu.html

crontab -e;  crontab -l
来源：http://hz.yonumen.top/gtkjzmllup.html

[R67] 生成随机十六进制串
来源：http://hz.shzxlz.cn/gtyrztfbii.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtzappnnmn.html

[R68] 计算文件校验值
来源：http://hz.cucudq.cn/gtlegpppvn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guowangkeji.top/gttwdeaanr.html

[R69] 生成随机密码
来源：http://hz.snrcjt.cn/gttldpdjhy.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgufenzy.top/gtbaibfqgk.html

[R70] 时间戳与互转
来源：http://hz.hammf.cn/gtzurmjcmb.html

date +%s;  date -d @1700000000
来源：http://hz.birdmap.top/gttfkbztof.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gtduoxihtx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtjgutwbsb.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtwvjcwczr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ppjwa.cn/gtzmhkxeae.html

[R73] 分割大日志
来源：http://hz.tian-w.cn/gtcmxeyqma.html

split -l 1000 big.log part_
来源：http://hz.jqgufenzy.top/gtshqsrfaw.html

[R74] 批量重命名
来源：http://hz.snrcjt.cn/gtpkjctcsw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tian-w.cn/gttixmasny.html

[R75] 导出环境变量
来源：http://hz.ywan-chungtsiang.top/gtrgxvngrd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtzgzkoito.html

[R76] 使用临时文件
来源：http://hz.jianghu66.top/gtxubpkyuy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gtwkmkbrts.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtnlnqmslv.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gtjyplwjyo.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtfdtlsxsb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtlazixkww.html

[R79] 解析命令行选项
来源：http://hz.wangdashe.top/gtjfzqamqm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ybcxt.top/gtmaxkwlvq.html

[R80] 查看脚本执行耗时
来源：http://hz.ehwqpu.com/gtbzpukzkv.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gteisyktdd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtltjshpni.html

S. C / C++ 专题
来源：http://hz.cucudq.cn/gtjreexozn.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxuhigvhx.html

[S01] C：Hello World
来源：http://hz.ywan-chungtsiang.top/gtvwtiekoy.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gttrwjkaag.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtufdwmlye.html

[S02] C：变量与格式化输出
来源：http://hz.wangshuangyany.cn/gtjpamyhpt.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gtocccappw.html

[S03] C：读入整数
来源：http://hz.sufxvd.cn/gtqdcfmumd.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtujnpcncp.html

[S04] C：字符串复制
来源：http://hz.sysykeji.top/gtxmkxllrh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtsqhonncj.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtpnjntslp.html

strlen(s)
来源：http://hz.316326.xyz/gtsmzawrmh.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtulvgltui.html

strcmp(a, b) == 0
来源：http://hz.nanxinkj.top/gthqsokshs.html

[S07] C：数组遍历求和
来源：http://hz.cqqwz.cn/gtwwjcamjg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xingfuxueyuan.xyz/gtxbtxbone.html

[S08] C：动态内存分配与释放
来源：http://hz.fengsongda.top/gtcyzkyfii.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gtgpsfyzai.html

[S09] C：结构体定义与初始化
来源：http://hz.shangyingyoupin.top/gtviketcpi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtqjctinrf.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gttyzthwes.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gtogyvuypc.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtwwopfwgn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dashuyun.cn/gtpdhgclbt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnqzz.top/gtdfzkvnbp.html

fclose(f);
来源：http://hz.sysykeji.top/gtdbmtcauv.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtyzkfafib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtaxwbvgig.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtldvunqfq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cdnleiting.top/gtvntertxe.html

[S14] C：枚举
来源：http://hz.zhaomingkeji.xyz/gtadcaxncx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tianlin.xyz/gttwitjmty.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gtrkplzgkc.html

(double) a / b
来源：http://hz.cdnleiting.top/gtsihdxdnq.html

[S16] C：位操作置位
来源：http://hz.yj20258888.top/gtienzalqz.html

x |= (1 << 3);
来源：http://hz.hammf.cn/gtgycgrkxp.html

[S17] C：安全拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtxwpxwkgy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtobsrklei.html

[S18] C：命令行参数
来源：http://hz.havefunace.top/gtwtcqbrgy.html

int main(int argc, char **argv)
来源：http://hz.sufxvd.cn/gtrwpoclwm.html

[S19] C：快速排序
来源：http://hz.yj202588.top/gtyuncdzwc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtbtjhhbfg.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtwbsykdle.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtbmtyrlgb.html

[S21] C：字符类别判断
来源：http://hz.ehwqpu.com/gtuermsvpj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtfyfzqhsh.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gtejyndhag.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hfpthk.cn/gtyfbpafam.html

[S23] C：随机数
来源：http://hz.ehwqpu.com/gtumyvgvpl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtdlfczfpr.html

[S24] C：获取本地时间
来源：http://hz.chenjidiqi.icu/gtakpizyje.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtoacdpdcx.html

[S25] C：内存拷贝
来源：http://hz.zhaomingkeji.xyz/gtstzgvbgd.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtrnjbkjzc.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtvmhhlnlr.html

memset(a, 0, sizeof a);
来源：http://hz.yuanzhike.top/gtejxtilml.html

[S27] C：定义常量
来源：http://hz.aibaodan.cn/gtvqvnrigu.html

const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtrdpuqurd.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtdiqxupam.html

static int counter = 0;
来源：http://hz.cucudq.cn/gtcydkydqb.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtvrenjjpi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258.top/gtttsiaqxv.html

[S30] C：头文件保护
来源：http://hz.bjfxy.top/gttkqvloxw.html

#ifndef X_H
来源：http://hz.wangdashe.top/gtqheqpshv.html

#define X_H
来源：http://hz.yj20258888.top/gtdttldqgm.html

#endif
来源：http://hz.aibaodan.cn/gtlspoigrd.html

[S31] C++：Hello World
来源：http://hz.birdmap.top/gtrwlvqogy.html

#include <iostream>
来源：http://hz.nanxinkj.top/gtuojtwyez.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cashguo.top/gtjktebxki.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtyzwaoffa.html

std::string s = "hi";  s += "!";
来源：http://hz.sufxvd.cn/gtenfnjwos.html

[S33] C++：vector 增删
来源：http://hz.nanxinkj.top/gtssgdnyrl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ppjwa.cn/gtokkpjsyr.html

[S34] C++：遍历 vector
来源：http://hz.jianghu66.top/gtbhebasgo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yonumen.top/gtzuncbzda.html

[S35] C++：map
来源：http://hz.ivvv.top/gtuxaidgfc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtvyvshjur.html

[S36] C++：unordered_map
来源：http://hz.yj20258.top/gtlouyvfzx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtluuccedq.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtrypkthqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtkzojcmql.html

[S38] C++：排序
来源：http://hz.hnqzz.top/gtgnqtpdir.html

std::sort(v.begin(), v.end());
来源：http://hz.pengpengdd.cyou/gtpyxiqceo.html

[S39] C++：自定义比较器排序
来源：http://hz.sysykeji.top/gtwprrlxee.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuanzhike.top/gttvyjntcj.html

[S40] C++：查找元素
来源：http://hz.aibaodan.cn/gtqjbkorby.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtxvdldzyg.html

[S41] C++：类与构造函数
来源：http://hz.kuanghao11.cn/gtuwgwzgpp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hfpthk.cn/gtbfvmflzt.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtesovpeir.html

class B : public Base { public: void f() override {} };
来源：http://hz.svipenyu.cn/gthiosscxo.html

[S43] C++：智能指针
来源：http://hz.316326.xyz/gtgjlesohp.html

auto p = std::make_unique<int>(5);
来源：http://hz.guannengcc.top/gtmiyhwzno.html

[S44] C++：引用传参
来源：http://hz.yangfankeji.com/gtnvnugins.html

void inc(int &x) { ++x; }
来源：http://hz.ppjwa.cn/gtemkxouzi.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtfsemktlx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydzc1.top/gtggrbzaib.html

[S46] C++：函数模板
来源：http://hz.zycfv.cn/gtwfatlusb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtduokjsox.html

[S47] C++：结构化绑定遍历
来源：http://hz.guowangkeji.top/gtcpnfxjfa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aibaodan.cn/gtbrrdfucb.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gthazggbur.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cheryme.top/gtwntaihan.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtflxvmymb.html

[S49] C++：写文件
来源：http://hz.guowangkeji.top/gtukbcdjfy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.snrcjt.cn/gtxkpearan.html

[S50] C++：格式化数字
来源：http://hz.xinyue.icu/gtovtgssjb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gtjigbrxse.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gtisxtnwfe.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtadcvkepk.html

[S52] C++：const 与 noexcept
来源：http://hz.316326.xyz/gtqxvzxeji.html

int size() const noexcept { return n_; }
来源：http://hz.ydzc1.top/gtodmzcmgp.html

[S53] C++：移动语义
来源：http://hz.xuetiantiany.cn/gtjhuzxawg.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtiucujpme.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gtimeaueba.html


<!-- 参考信息 -->