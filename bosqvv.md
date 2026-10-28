代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtrdmhyfqd.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtzfgcemov.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gthkgzjbzu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtmqvrfvtj.html

[Q86] 读取 JSON 字段
来源：http://hz.yonumen.top/gtbwoqnpur.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gtnppapevu.html

[Q87] JSON 字段做条件
来源：http://hz.redwolf501.top/gtpoxvqofh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtdyuwuhiw.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtwnofchup.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.birdmap.top/gtmlartpxh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhongyouzk.top/gthgpfsnnv.html

[Q89] 判断表是否存在
来源：http://hz.pengpengdd.cyou/gtabgujkol.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangtech.top/gtsfoeofca.html

[Q90] 生成序号列
来源：http://hz.kuanghao11.cn/gtpyooufcr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zdqjudy.top/gtvlxpqwzj.html

================================================================================
来源：http://hz.daxiang520.top/gtqtzwgasw.html

R. Bash 专题
来源：http://hz.hammf.cn/gtxzmwiyrp.html

================================================================================
来源：http://hz.redwolf501.top/gtzwtrgqpj.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtvxjwkhdv.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtvyjvdcel.html

set -euo pipefail
来源：http://hz.ydjk.org.cn/gtcqgfgewx.html

[R02] 变量赋值与使用
来源：http://hz.wangshuangyany.cn/gteoglzpfz.html

name="Tom"; echo "$name"
来源：http://hz.haohaochexian.top/gtjzkcbfme.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtehjguuyw.html

readonly PI=3.14
来源：http://hz.cheryme.top/gtekkbhawg.html

[R04] 位置参数
来源：http://hz.jiagoushi.top/gtudbpghmh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gttavjvoeu.html

[R05] 参数默认值
来源：http://hz.tanke756.top/gtxugefrop.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtcsguavxx.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtawlkboyq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.svipenyu.cn/gtaserorxh.html

[R07] if 判断文件
来源：http://hz.52xcode.cn/gtcresnebs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtlkpuwwtu.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtmxpapnmw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigfzy.top/gtekuorrvp.html

[R09] 字符串比较
来源：http://hz.pycfn.com/gtavfvlomd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtwpronbqm.html

[R10] 正则匹配
来源：http://hz.316326.xyz/gtxrxjdjvq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aizwys.cn/gtnglhxfvr.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtkzvrfskg.html

case "$1" in
来源：http://hz.jinghuilouyu.cn/gtgfmsupqj.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtqdntkhzn.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtzktcmjgf.html

*)     echo "未知命令" ;;
来源：http://hz.hfpthk.cn/gtomxeisye.html

esac
来源：http://hz.sufxvd.cn/gtmhrrqoic.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtectuoizc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuetiantiany.cn/gttswnhnfd.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gtedjiiqyr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.smart0.xyz/gthsbutngx.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtlvtlngjs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtzbuqoblj.html

[R15] while 逐行读文件
来源：http://hz.jinqigufen.top/gtscgijpti.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hongshengwenyu.top/gtktaqpjxr.html

[R16] until 等待条件
来源：http://hz.shuidangran.top/gtwsmpahpi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.meibo888.top/gtsxzrkmxv.html

[R17] 数组定义与取值
来源：http://hz.mhx1999.top/gtguwnbxcc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yonumen.top/gttwuehsdo.html

[R18] 遍历数组
来源：http://hz.c1oappe.top/gtftqfnezg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yangfankeji.com/gtmivuuvmb.html

[R19] 数组长度
来源：http://hz.nanxuanxn.top/gtuaoojnjr.html

echo "${#arr[@]}"
来源：http://hz.hfpthk.cn/gtsjguimtt.html

[R20] 关联数组（字典）
来源：http://hz.gzhubu.top/gtuddlyykg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yanxiufei.cn/gtuegdfiud.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtbiwxzmwp.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtlpyehjpw.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gtrgeyebpg.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtzrnosimz.html

[R23] 字符串替换
来源：http://hz.cashguo.top/gtlshnlkfm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haohaochexian.top/gtdnxhksdh.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtjrqrunvj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yuxming.cn/gtnulgnlof.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gtnelyfthx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtravgweia.html

[R26] 命令替换
来源：http://hz.daxiang520.top/gtrkndesau.html

now=$(date +%F); echo "$now"
来源：http://hz.redwolf501.top/gtkvgmrhdj.html

[R27] 算术展开
来源：http://hz.jinyuanbaomall.cn/gtxuvcfmgr.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtmoedlmbt.html

[R28] 浮点运算
来源：http://hz.sweek.top/gtxbmxhasx.html

echo "scale=2; 10/3" | bc
来源：http://hz.guannengcc.top/gtrrbinqlx.html

[R29] 定义函数
来源：http://hz.smart0.xyz/gtuzaixgeo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtcnayfmql.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtvepwdcgt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhoulong.xyz/gthbavfabe.html

[R31] 局部变量
来源：http://hz.jqgfzy.top/gtnkkjkqmq.html

f() { local x=1; echo "$x"; }
来源：http://hz.gotoacloud.top/gtupejrwmj.html

[R32] 参数个数校验
来源：http://hz.ydjk.org.cn/gtrotoqzxq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fengsongda.top/gttopssedz.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtmerthuhk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtxwcxbrub.html

[R34] 退出时清理
来源：http://hz.pengpengdd.cyou/gtdljbtfgw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtouskhchs.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtqtxmkcbg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtsdkcqefp.html

[R36] 并发执行多个任务
来源：http://hz.jqgfzy.top/gtzgviuzmo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aibaodan.cn/gtfvdpbvab.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangtech.top/gtqyanothf.html

files=$(ls -1)
来源：http://hz.feifeiyinyue.top/gtnunqorfp.html

[R38] 管道串联
来源：http://hz.xylfe.cn/gtelgfdimv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydjk.org.cn/gtcijtzrhi.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtbltghwob.html

cmd > out.log 2>&1
来源：http://hz.sxryk.cn/gtmwslungb.html

[R40] 追加写日志
来源：http://hz.chenlongwang.top/gtpmqfprfu.html

echo "log" >> out.log
来源：http://hz.316326.xyz/gtosagmnfj.html

[R41] 丢弃输出
来源：http://hz.xuanzx.com/gtmujqokpx.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigfzy.top/gtgupqgvrh.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtrcrffbav.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gttholngls.html

[R43] 按名字查找文件
来源：http://hz.hnxiangtu.top/gtwhkafgfq.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gttrvzevnv.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtyjlimuiy.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtovcavurx.html

[R45] 批量删除
来源：http://hz.haohaochexian.top/gthhgwdifo.html

find . -name "*.tmp" -delete
来源：http://hz.hfpthk.cn/gtpwblcejl.html

[R46] 递归替换文件内容
来源：http://hz.snrcjt.cn/gtlidhqxij.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gtjpbobiyw.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtxbzifcyi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gtyrfuwrzv.html

[R48] awk 取指定列
来源：http://hz.zycfv.cn/gtcsvbxhwz.html

awk '{print $1, $3}' a.txt
来源：http://hz.hfpthk.cn/gtruqfziuu.html

[R49] awk 带条件
来源：http://hz.hongshengwenyu.top/gtkzjzfbkg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gthqfhlkcn.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtbasbubxm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtvvassjxj.html

[R51] 排序去重取前几
来源：http://hz.jinyuanbaomall.cn/gtodmhzuzi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtmivbeuzd.html

[R52] 统计行数
来源：http://hz.hnqzz.top/gtvhjgicew.html

wc -l a.txt
来源：http://hz.dashuyun.cn/gtcxlakscv.html

[R53] 查看文件头与实时尾
来源：http://hz.fengsongda.top/gtvqomlxbk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gthpetwenc.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtbmmxneqg.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtcoardntg.html

[R55] 压缩与解压
来源：http://hz.yvedp.cn/gtjjqahqly.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gtwhwluhqc.html

[R56] 远程拷贝
来源：http://hz.nanxuanxn.top/gtjtfukuar.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtghqllelk.html

[R57] 远程执行命令
来源：http://hz.ydjk.org.cn/gtnbuovkrr.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtkidttsyt.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtwiaiftcy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtcvvhtpwl.html

[R59] 发 POST JSON
来源：http://hz.fengsongda.top/gtkaafkvim.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhoulong.xyz/gtpmcyiqjq.html

[R60] 只看 HTTP 状态码
来源：http://hz.tanke756.top/gtfsphivpr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtiabhoymn.html

[R61] 磁盘占用
来源：http://hz.jqgufenzy.top/gtbraafzib.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtxnoanyea.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtcpgyympj.html

du -ah . | sort -rh | head -10
来源：http://hz.gotoacloud.top/gtdyjredet.html

[R63] 内存与进程
来源：http://hz.ppjwa.cn/gtmeqpxrpc.html

free -h;  ps aux | grep nginx
来源：http://hz.quarkkingdee.top/gtsmazsuoi.html

[R64] 结束进程
来源：http://hz.316326.xyz/gtihgqppkm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtunkinjia.html

[R65] 查看端口占用
来源：http://hz.fzhhl.top/gtkzgziuns.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.feifeiyinyue.top/gtjzcvlkxn.html

[R66] 定时任务
来源：http://hz.yangfankeji.com/gtcfayhnau.html

crontab -e;  crontab -l
来源：http://hz.hammf.cn/gtztprhpfw.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtcvylnzud.html

openssl rand -hex 16
来源：http://hz.tanke756.top/gtffwltgbp.html

[R68] 计算文件校验值
来源：http://hz.jqgufenzy.top/gtocgblppb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtrepzueuj.html

[R69] 生成随机密码
来源：http://hz.daria6918.cn/gtevfzljze.html

head -c 16 /dev/urandom | base64
来源：http://hz.havefunace.top/gthebfqzok.html

[R70] 时间戳与互转
来源：http://hz.gogol.net.cn/gtjuarmtfg.html

date +%s;  date -d @1700000000
来源：http://hz.zhaomingkeji.xyz/gtkbbspfca.html

[R71] 日期格式化
来源：http://hz.svipenyu.cn/gtmfyrhsbg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigfzy.top/gthdywsydj.html

[R72] 等待端口就绪
来源：http://hz.yonumen.top/gtltujzcit.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.316326.xyz/gtzvhjzyxw.html

[R73] 分割大日志
来源：http://hz.shangyingyoupin.top/gtryshbriu.html

split -l 1000 big.log part_
来源：http://hz.hnxiangtu.top/gtiavkjcpu.html

[R74] 批量重命名
来源：http://hz.gaohongyu789.top/gtoxisduer.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gtxgqexupc.html

[R75] 导出环境变量
来源：http://hz.nanxinkj.top/gtqfxsiphm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtwdkeeqcg.html

[R76] 使用临时文件
来源：http://hz.zhixingplan.top/gthhegiwfr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtyydelhdb.html

[R77] 读取用户输入
来源：http://hz.zhongyouzk.top/gtnoktqdps.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtsuwpxmfh.html

[R78] 交互式菜单
来源：http://hz.xuanzx.com/gtiznlgpeh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gogol.net.cn/gthybkuzmm.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gticpjztee.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ehwqpu.com/gtkmjsdzjg.html

[R80] 查看脚本执行耗时
来源：http://hz.zhixingplan.top/gtusmgsigy.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gtemnwfyci.html

================================================================================
来源：http://hz.sufxvd.cn/gtqybdfaoc.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtmwlpyuit.html

================================================================================
来源：http://hz.zdqjudy.top/gtzgshfipf.html

[S01] C：Hello World
来源：http://hz.xingfuxueyuan.xyz/gttgrhziwd.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtfwzdiwtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ivvv.top/gtqvjuchjy.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtqsqscutu.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gtobihhqar.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gtkkajwfbl.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtskaepjpy.html

[S04] C：字符串复制
来源：http://hz.yangfankeji.com/gtojwcplug.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtdoyvwnzk.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gtpvsadska.html

strlen(s)
来源：http://hz.dashuyun.cn/gtkhedfgfn.html

[S06] C：字符串比较
来源：http://hz.c1oappe.top/gtsdvqqfcw.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtwvjgqazr.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gteisvzjpa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.quarkkingdee.top/gtzxftcapp.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtqlhwjqzf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtqwregxoc.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gtvbadpqgq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pengpengdd.cyou/gtdvsgitmx.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gtevruxhca.html

int *p = &a;  *p = 5;
来源：http://hz.yanxiufei.cn/gtgxuizqqk.html

[S11] C：逐行读文件
来源：http://hz.yj20258888.top/gtipqyvwoo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zycfv.cn/gthwrklnsv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.quarkkingdee.top/gtrdfclkon.html

fclose(f);
来源：http://hz.zhijiandao.cn/gtjkiayovy.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gthtvouwfa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtazaazswh.html

[S13] C：宏定义
来源：http://hz.xinyue.icu/gtqxiedjqu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cheryme.top/gttypnaakz.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtnvcdrcwm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.redwolf501.top/gtwwbsrowj.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtdettbyzj.html

(double) a / b
来源：http://hz.hnqzz.top/gtbrtsnwgl.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gticqngsdo.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtpebpkrzl.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtovfzcnay.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydjk.org.cn/gtnmiraoxv.html

[S18] C：命令行参数
来源：http://hz.chenlongwang.top/gtgzjfquon.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtqcaluhjt.html

[S19] C：快速排序
来源：http://hz.meibo888.top/gtmpdmthtn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtwgyonngh.html

[S20] C：二分查找
来源：http://hz.hfpthk.cn/gtldnnhfsh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtcegfuyvp.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtnkggvmwj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtcnktxhgh.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtrfotiaxb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtmozqrxcl.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtbovdukbs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guowangkeji.top/gttvyowise.html

[S24] C：获取本地时间
来源：http://hz.xylfe.cn/gtxhrfkppo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.meibo888.top/gtihfpmati.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtuqbdrlox.html

memcpy(dst, src, n);
来源：http://hz.jlsjyb.cn/gtumkdbglk.html

[S26] C：内存清零
来源：http://hz.pengpengdd.cyou/gtqsghaxss.html

memset(a, 0, sizeof a);
来源：http://hz.chenzaomai.com/gtfrtbhjbf.html

[S27] C：定义常量
来源：http://hz.chenzaomai.com/gtikkvhrxg.html

const double PI = 3.14159;
来源：http://hz.sysykeji.top/gtumpmmcyl.html

[S28] C：静态变量
来源：http://hz.redwolf501.top/gtelasbxrl.html

static int counter = 0;
来源：http://hz.gzhubu.top/gtdtszdcdm.html

[S29] C：变参函数
来源：http://hz.c1oappe.top/gtdfiuezeb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtfhkujaak.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtbwkqdtmx.html

#ifndef X_H
来源：http://hz.jinqigufen.top/gtftogcovf.html

#define X_H
来源：http://hz.xziqi.cn/gtgdpqpyfo.html

#endif
来源：http://hz.tanke756.top/gtzlvotmaz.html

[S31] C++：Hello World
来源：http://hz.zhixingplan.top/gtndzwvdsk.html

#include <iostream>
来源：http://hz.yvedp.cn/gtppbvpmjo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangkeji.top/gtcwckmuyg.html

[S32] C++：字符串
来源：http://hz.tian-w.cn/gtihecvqhw.html

std::string s = "hi";  s += "!";
来源：http://hz.xuetiantiany.cn/gtelegxvqt.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtkjeryayo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtjydpavgg.html

[S34] C++：遍历 vector
来源：http://hz.ehwqpu.com/gtsnfmjvvq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.andypj.xyz/gtokrlkhfa.html

[S35] C++：map
来源：http://hz.haohaochexian.top/gtozyyzvqd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtkfajdppm.html

[S36] C++：unordered_map
来源：http://hz.xingfuxueyuan.xyz/gthntskses.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtqxvhkjjj.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gteohiakxf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.9152youxi.cn/gtyoajdoga.html

[S38] C++：排序
来源：http://hz.yj20258.top/gtpwrxbfqa.html

std::sort(v.begin(), v.end());
来源：http://hz.chenjidiqi.icu/gtbtbnoyqr.html

[S39] C++：自定义比较器排序
来源：http://hz.jianghu66.top/gtdrbgsytm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.birdmap.top/gthwzwzlur.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gtusdlgras.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtkndzquwc.html

[S41] C++：类与构造函数
来源：http://hz.jinqigfzy.top/gtfpvdirje.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xinyue.icu/gthplsjwnb.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtztnleuqi.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuetiantiany.cn/gtofneajrg.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtbtsswzvz.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtcohoscod.html

[S44] C++：引用传参
来源：http://hz.yanxiufei.cn/gtowlvqrdx.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtuwvfeslx.html

[S45] C++：lambda
来源：http://hz.iojbl.cn/gttunipjvi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtydgmsxdu.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtfsdtzphk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhaomingkeji.xyz/gtdzblvmej.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuanzx.com/gtpqlukzce.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yonumen.top/gtygehhjvg.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtvkvlfjpt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ywan-chungtsiang.top/gtyythalxv.html

while (std::getline(in, line)) { }
来源：http://hz.gaohongyu789.top/gthnymaubm.html

[S49] C++：写文件
来源：http://hz.jyoumei.cn/gtszdcqula.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.kuanghao11.cn/gtcnwzqeqt.html

[S50] C++：格式化数字
来源：http://hz.jianghu66.top/gtacztxwgz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.kuanghao11.cn/gtqdfabzek.html

[S51] C++：显式类型转换
来源：http://hz.yonumen.top/gtggwhrros.html

static_cast<double>(a) / b
来源：http://hz.yongpay.top/gttazfcoji.html

[S52] C++：const 与 noexcept
来源：http://hz.fengsongda.top/gtkysybptw.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangkeji.top/gtdooosnfh.html

[S53] C++：移动语义
来源：http://hz.jiagoushi.top/gtwqagvxia.html

std::vector<int> w = std::move(v);
来源：http://hz.svipenyu.cn/gtvasbxwex.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gthnjqywql.html


<!-- 参考信息 -->