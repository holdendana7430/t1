代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gtglzrdaei.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtjjwxxwpn.html

[Q87] JSON 字段做条件
来源：http://hz.dianchejie.cn/gtufvpwmnd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtikzmriwq.html

[Q88] 行转列（条件聚合）
来源：http://hz.guowangkeji.top/gtubmqcxmr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yonumen.top/gtejbdzjwt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtsexjkvuj.html

[Q89] 判断表是否存在
来源：http://hz.nanxinkj.top/gtvbrxtawm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtlofgiupc.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gtztqecpqs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtcoajctjg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtsmzsfpap.html

R. Bash 专题
来源：http://hz.cqqwz.cn/gtnqrajadv.html

================================================================================
来源：http://hz.shzxlz.cn/gtjoalvmdg.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gtlibqxehg.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtamecxddc.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtfvjutduj.html

[R02] 变量赋值与使用
来源：http://hz.zhixingplan.top/gtxmgnejjx.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtskeztukf.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtlhsdwnrh.html

readonly PI=3.14
来源：http://hz.bjfxy.top/gtvfhdowkp.html

[R04] 位置参数
来源：http://hz.jinqigufen.top/gtbhpfarbb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtgogsbmkk.html

[R05] 参数默认值
来源：http://hz.shanyushiyangkeji.top/gttokpvqap.html

name="${1:-default}"
来源：http://hz.zhengqikj.top/gtpvxnoumr.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gtwabaiqyr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhengqikj.top/gttoswthtn.html

[R07] if 判断文件
来源：http://hz.sxryk.cn/gtdgbusgyc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gtuwfqnrqw.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtpbjjpehb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhiwuduotai.top/gtzmyprvam.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gtgnwvgspj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.kuanghao11.cn/gtuarizggw.html

[R10] 正则匹配
来源：http://hz.ppjwa.cn/gthjhgdgkm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ydjk.org.cn/gtrfiygack.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtrconyvcx.html

case "$1" in
来源：http://hz.sweek.top/gtrntynjib.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtejjramlj.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gttxvjkqpf.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtqluwdqyj.html

esac
来源：http://hz.quarkkingdee.top/gtfnnkftpx.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtyikyfavv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenjidiqi.icu/gtrumcwymy.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtecbsvgnj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtccwbmzzx.html

[R14] C 风格 for
来源：http://hz.hnqzz.top/gtfdngchpx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gttzjzplaw.html

[R15] while 逐行读文件
来源：http://hz.hfpthk.cn/gtrentarmt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cqqwz.cn/gttpgbukrd.html

[R16] until 等待条件
来源：http://hz.zhongyouzk.top/gtmjwgveoy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenlongwang.top/gtjodqulrt.html

[R17] 数组定义与取值
来源：http://hz.52xcode.cn/gtuupgrmhr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtsnrvukly.html

[R18] 遍历数组
来源：http://hz.guowangkeji.top/gteqopxguk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gtxfisvcao.html

[R19] 数组长度
来源：http://hz.xinyue.icu/gtovnckgyp.html

echo "${#arr[@]}"
来源：http://hz.c1oappe.top/gtgnntjkls.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gtclqxylbc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtfqgzsxus.html

[R21] 字符串长度
来源：http://hz.hfpthk.cn/gtisdrmjzt.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtkhnxppcw.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gtxuceqpbi.html

echo "${s:0:5}"
来源：http://hz.dianchejie.cn/gtmqnehwqe.html

[R23] 字符串替换
来源：http://hz.cucudq.cn/gtemspjooy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gthxgmzetb.html

[R24] 大小写转换
来源：http://hz.gotoacloud.top/gtnlmxvyva.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gtqycuwtth.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtiuemaqtz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gaohongyu789.top/gttthhpuig.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtnrhdekmu.html

now=$(date +%F); echo "$now"
来源：http://hz.zhiwuduotai.top/gtrypxlmjf.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gttdvfzczp.html

echo $((1 + 2 * 3))
来源：http://hz.jinghuilouyu.cn/gteqmydsdt.html

[R28] 浮点运算
来源：http://hz.52xcode.cn/gtzxbfeidv.html

echo "scale=2; 10/3" | bc
来源：http://hz.jiagoushi.top/gtmvsggyzy.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gtridoytnv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnxiangtu.top/gtzfghfult.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtfmpzjdzz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.snrcjt.cn/gtkhyqvtbb.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gtozivkbsn.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtfuxsfqgz.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtvfeqbgpy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.kuanghao11.cn/gtmjjpuppu.html

[R33] 捕获错误并提示行号
来源：http://hz.aizwys.cn/gtwzaoqxqe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gtvdpsloqy.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtreuhhsxu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtbgskpadd.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gthqgxwobt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhongyouzk.top/gtkrjmepyk.html

[R36] 并发执行多个任务
来源：http://hz.tian-w.cn/gtvoyjuzmt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fengsongda.top/gttuvglofy.html

[R37] 把输出赋给变量
来源：http://hz.dianchejie.cn/gtcygmzuci.html

files=$(ls -1)
来源：http://hz.yuxming.cn/gtgmjabefo.html

[R38] 管道串联
来源：http://hz.zdqjudy.top/gtikkoxfrk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtqyklspak.html

[R39] 重定向标准输出与错误
来源：http://hz.yvedp.cn/gtsfxtmset.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gtenwgvfce.html

[R40] 追加写日志
来源：http://hz.pycfn.com/gtnvfmptgx.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtejbzqwdp.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtzqmjroxa.html

cmd >/dev/null 2>&1
来源：http://hz.pengpengdd.cyou/gtyeakzhic.html

[R42] 输入重定向
来源：http://hz.sxryk.cn/gtdfjqkqmf.html

wc -l < a.txt
来源：http://hz.dianchejie.cn/gtrhufxfop.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gthkqttdcq.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtfmffcgvc.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gttbrunatp.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtijvvewda.html

[R45] 批量删除
来源：http://hz.ywan-chungtsiang.top/gtzlysqthj.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtfgfgzvvb.html

[R46] 递归替换文件内容
来源：http://hz.zhoulong.xyz/gtykxuevmx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gtcdapnjvd.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtpyyldvxy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtbxbjajju.html

[R48] awk 取指定列
来源：http://hz.yangfankeji.com/gtwiuinqlg.html

awk '{print $1, $3}' a.txt
来源：http://hz.cdnleiting.top/gtqeyqkfaj.html

[R49] awk 带条件
来源：http://hz.zhixingplan.top/gtfvtqphpx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.quarkkingdee.top/gtrdhwupyp.html

[R50] awk 求和
来源：http://hz.cashguo.top/gthpssoqfe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenjidiqi.icu/gtlmslknpx.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtieaojpsf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenlongwang.top/gtqpplybit.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtqrsgqrgx.html

wc -l a.txt
来源：http://hz.yj202588.top/gthioofhiy.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtmomtqjht.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xingfuxueyuan.xyz/gtsybuwhnf.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gtkspbzxev.html

diff a.txt b.txt
来源：http://hz.shangyingyoupin.top/gtfzwuwbqg.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtbbkpjlql.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ywan-chungtsiang.top/gtrzeoqzbf.html

[R56] 远程拷贝
来源：http://hz.gzhubu.top/gtnlpciedc.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gthffdrlof.html

[R57] 远程执行命令
来源：http://hz.dashuyun.cn/gtwdzeuggo.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtmbnoyrsf.html

[R58] 下载文件
来源：http://hz.jinyuanbaomall.cn/gtpjvphywl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnqzz.top/gtvpdwitmi.html

[R59] 发 POST JSON
来源：http://hz.jqgufenzy.top/gtqlmclyue.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtmgimnyho.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtgybjjxmi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cashguo.top/gtqrcehujk.html

[R61] 磁盘占用
来源：http://hz.daxiang520.top/gtdbedyiol.html

df -h;  du -sh *
来源：http://hz.0kj1m.cn/gtcpvhkpjc.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtgndsckcd.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtlrtvbnjr.html

[R63] 内存与进程
来源：http://hz.dashuyun.cn/gtyuumwabc.html

free -h;  ps aux | grep nginx
来源：http://hz.zhoulong.xyz/gtkovoeznn.html

[R64] 结束进程
来源：http://hz.mhx1999.top/gtoflczdgh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.iojbl.cn/gtitwlytvo.html

[R65] 查看端口占用
来源：http://hz.chenzaomai.com/gtcxbjypaq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangtech.top/gtexvrpbox.html

[R66] 定时任务
来源：http://hz.mhx1999.top/gtctovwnfh.html

crontab -e;  crontab -l
来源：http://hz.dashuyun.cn/gtskjpznuk.html

[R67] 生成随机十六进制串
来源：http://hz.sysykeji.top/gtvhskmfqc.html

openssl rand -hex 16
来源：http://hz.jinyuanbaomall.cn/gtnisladqh.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtdzieiyoq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gtghelpnzw.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gtzxcjmboz.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenjidiqi.icu/gtwouuesdo.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtesbcnpcf.html

date +%s;  date -d @1700000000
来源：http://hz.gaohongyu789.top/gtztzxwepl.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtnzvvxmvz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtgtberxxn.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtmlciibff.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtnazzqnov.html

[R73] 分割大日志
来源：http://hz.hnxiangtu.top/gtaghccdbd.html

split -l 1000 big.log part_
来源：http://hz.ydzc1.top/gtzjqhilfl.html

[R74] 批量重命名
来源：http://hz.ivvv.top/gtygkehpvn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtviotixgg.html

[R75] 导出环境变量
来源：http://hz.nanxuanxn.top/gtujzmhuhz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtjngizhsi.html

[R76] 使用临时文件
来源：http://hz.shzxlz.cn/gtkteibyoj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtrawtypxo.html

[R77] 读取用户输入
来源：http://hz.gzhubu.top/gtyhhoqaok.html

read -rp "请输入: " ans
来源：http://hz.xingfuxueyuan.xyz/gtkmtotmxj.html

[R78] 交互式菜单
来源：http://hz.meibo888.top/gttabyqqki.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtwyodvnqw.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtdsmoewzu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtymqsaqnn.html

[R80] 查看脚本执行耗时
来源：http://hz.hammf.cn/gtxrgaflss.html

time ./run.sh
来源：http://hz.zhoulong.xyz/gtzlxrggxi.html

================================================================================
来源：http://hz.jinqigufen.top/gtfscyvstr.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gthnhbvhtv.html

================================================================================
来源：http://hz.sysykeji.top/gtztphbsdi.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtxtgrnbno.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtykoeydqh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtdhpnblgs.html

[S02] C：变量与格式化输出
来源：http://hz.feifeiyinyue.top/gtbegwqvbz.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenlongwang.top/gtspkbbcvj.html

[S03] C：读入整数
来源：http://hz.yj20258888.top/gtuoprokec.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gtdyfaewen.html

[S04] C：字符串复制
来源：http://hz.jlsjyb.cn/gtdoglfagi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtisfkmgea.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtujxnzijd.html

strlen(s)
来源：http://hz.dianchejie.cn/gtclibsljt.html

[S06] C：字符串比较
来源：http://hz.yanxiufei.cn/gthpwyisgf.html

strcmp(a, b) == 0
来源：http://hz.jinyuanbaomall.cn/gtvghkobqo.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtnjrmmrgc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daxiang520.top/gthqpnzwem.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtfxxvaruo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtjrpstszy.html

[S09] C：结构体定义与初始化
来源：http://hz.aibaodan.cn/gtrjbiaonv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gotoacloud.top/gtbyymuphy.html

[S10] C：指针与解引用
来源：http://hz.tanke756.top/gtlkodapst.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258.top/gttavmhvpc.html

[S11] C：逐行读文件
来源：http://hz.hongshengwenyu.top/gtpdvgvsis.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtwnsqxaac.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gttygkdrcn.html

fclose(f);
来源：http://hz.xziqi.cn/gtzivqqfio.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtzdrsapef.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhixingplan.top/gtbmunqjdq.html

[S13] C：宏定义
来源：http://hz.haohaochexian.top/gtzpkuokbm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtxzsvnidr.html

[S14] C：枚举
来源：http://hz.pycfn.com/gtrctzyins.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtzzolvrgd.html

[S15] C：类型转换
来源：http://hz.hywenlv.cn/gtypnofnui.html

(double) a / b
来源：http://hz.9152youxi.cn/gtaixlkqne.html

[S16] C：位操作置位
来源：http://hz.feifeiyinyue.top/gtlatxltsg.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtqedaocer.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtfxudtzmt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hysaishi.cn/gtlrdxftfg.html

[S18] C：命令行参数
来源：http://hz.quarkkingdee.top/gtsurdnszj.html

int main(int argc, char **argv)
来源：http://hz.xinyue.icu/gtxuymbogu.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gtlbremprl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtfpeqnlth.html

[S20] C：二分查找
来源：http://hz.jlsjyb.cn/gtszyaykyo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gthoegwdso.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtbjhcbifx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtjsvxxixc.html

[S22] C：字符串转数字
来源：http://hz.jinqigufen.top/gtrovpkabn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.bjfxy.top/gtdmtgdxyg.html

[S23] C：随机数
来源：http://hz.xingfuxueyuan.xyz/gtqmwuyshd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydjk.org.cn/gtlsgnownj.html

[S24] C：获取本地时间
来源：http://hz.316326.xyz/gtjrgnohsx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhongyouzk.top/gtupydmtuk.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtumllmfek.html

memcpy(dst, src, n);
来源：http://hz.daria6918.cn/gtphpypegq.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtqscsaauf.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gtjligsmjw.html

[S27] C：定义常量
来源：http://hz.tanke756.top/gtcxzffncu.html

const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtdoipwbgw.html

[S28] C：静态变量
来源：http://hz.chenlongwang.top/gtkbcunrzz.html

static int counter = 0;
来源：http://hz.jqgfzy.top/gtkzvqzdrw.html

[S29] C：变参函数
来源：http://hz.wangshuangyany.cn/gtvqxdzvrt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtgqzktwnr.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtiwnfcnhu.html

#ifndef X_H
来源：http://hz.nanxinkj.top/gtlclvirek.html

#define X_H
来源：http://hz.zdqjudy.top/gteebylzxs.html

#endif
来源：http://hz.gzhubu.top/gtxrjjnjtz.html

[S31] C++：Hello World
来源：http://hz.ybcxt.top/gtjmerxlxv.html

#include <iostream>
来源：http://hz.smart0.xyz/gtjefloqok.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gttuaptpvh.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gtoelussxq.html

std::string s = "hi";  s += "!";
来源：http://hz.hnqzz.top/gtlhbhvpyr.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gttfbccqcz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.svipenyu.cn/gtkzytadft.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtqmdemtqj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtocpfgojr.html

[S35] C++：map
来源：http://hz.cheryme.top/gtmvrpbcqi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtdbxnosoi.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gthrqbqnmx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtnvdokxul.html

[S37] C++：set
来源：http://hz.yj202588.top/gtjiicmvac.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gthkbqybat.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtvuctwibk.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gtpbrqyjdb.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gtctzcvtnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tanke756.top/gtwqfcvput.html

[S40] C++：查找元素
来源：http://hz.redwolf501.top/gthepplvgy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jiagoushi.top/gtmzkgfuvj.html

[S41] C++：类与构造函数
来源：http://hz.pycfn.com/gtqwhmplus.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtqwtxcvpu.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangtech.top/gtniytdedo.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtpdaiqmzk.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtzvfmsidw.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinqigfzy.top/gtmppqhgpn.html

[S44] C++：引用传参
来源：http://hz.jqgfzy.top/gtnmsroubw.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtiwgmaytk.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gtknkrlfon.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtwvollslx.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtzqyseyxp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yueranfly.top/gteftymdka.html

[S47] C++：结构化绑定遍历
来源：http://hz.yvedp.cn/gtxmnarkur.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinghuilouyu.cn/gtjhbatjko.html

[S48] C++：逐行读文件
来源：http://hz.chenzaomai.com/gtciqosjyw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gtxjsfcotq.html

while (std::getline(in, line)) { }
来源：http://hz.pycfn.com/gthhtcylqy.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtziviblaf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtxmfzpjxc.html

[S50] C++：格式化数字
来源：http://hz.jianghu66.top/gtzfhnpqkm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hysaishi.cn/gtkovihlwp.html

[S51] C++：显式类型转换
来源：http://hz.birdmap.top/gtmengynnu.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtevqtizaq.html

[S52] C++：const 与 noexcept
来源：http://hz.c1oappe.top/gtfodyliri.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtzkynihsm.html

[S53] C++：移动语义
来源：http://hz.smart0.xyz/gtpznkdvgn.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtoxcngvrb.html

[S54] C++：异常处理
来源：http://hz.guannengcc.top/gtovcbwdop.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.redwolf501.top/gtyocvogju.html

[S55] C++：结构化绑定
来源：http://hz.wangdashe.top/gttturebqn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.andypj.xyz/gtjfcayomh.html

[S56] C++：optional
来源：http://hz.zycfv.cn/gtdmllrtep.html


<!-- 参考信息 -->