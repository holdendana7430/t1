代发 wailian999

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtxbzxaofi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xziqi.cn/gtiycvcpqi.html

[Q77] 时间加减
来源：http://hz.aizwys.cn/gtjmunmwce.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtpqvoxajz.html

[Q78] 当前时间
来源：http://hz.nwbrower.top/gtzgnnudhc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtwwvwfecv.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtqyrxrnmw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gotoacloud.top/gtnedhvkzu.html

[Q80] 字符串截取
来源：http://hz.zhengqikj.top/gteeitjqpe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtxxwnctbr.html

[Q81] 字符串替换
来源：http://hz.zhijiandao.cn/gtjavqylhm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtilnfvegd.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtgtapcutc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtryaeoeqa.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtssyhowss.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtulxytkfh.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtzdrwvuvx.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtyzqgeqll.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtyyuarkyw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj202588.top/gtxhnwqtxc.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtxkxieyrd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtlvkljakl.html

[Q87] JSON 字段做条件
来源：http://hz.zhijiandao.cn/gtdtpaoinc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtmkgaxucs.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxinkj.top/gtcnkryldu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dianchejie.cn/gtzrydsljf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtpuaedtsl.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gtezxtfzfl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtrecxprej.html

[Q90] 生成序号列
来源：http://hz.feifeiyinyue.top/gtvzoczvgl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtpoqzcwsc.html

================================================================================
来源：http://hz.0kj1m.cn/gtwrnmvsbl.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtvcmawjvo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbchnklje.html

[R01] shebang 与严格模式
来源：http://hz.meibo888.top/gtzxoarela.html

#!/usr/bin/env bash
来源：http://hz.xylfe.cn/gthqlvbdnh.html

set -euo pipefail
来源：http://hz.sweek.top/gtiuktvhaq.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtphtxnupz.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtogqvrvsz.html

[R03] 只读变量
来源：http://hz.zdqjudy.top/gtqintntsx.html

readonly PI=3.14
来源：http://hz.jianghu66.top/gtifejfajt.html

[R04] 位置参数
来源：http://hz.jlsjyb.cn/gtqzeecemg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sysykeji.top/gthvkcamiy.html

[R05] 参数默认值
来源：http://hz.shanyushiyangkeji.top/gtuoxbbahe.html

name="${1:-default}"
来源：http://hz.zhixingplan.top/gtpcsuhcqz.html

[R06] 判断命令是否存在
来源：http://hz.guowangkeji.top/gtrmqjisjj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtrxtgoxmq.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtncjjusjg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtkvivmmrr.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gttjduyfop.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.havefunace.top/gtdvwyxxce.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtdsnpzogz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtrrawyyxn.html

[R10] 正则匹配
来源：http://hz.cashguo.top/gtizfyrcfm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gtvchdcrli.html

[R11] case 多分支
来源：http://hz.haohaochexian.top/gtycluiyzq.html

case "$1" in
来源：http://hz.yueranfly.top/gtdeoqcdwo.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gttlrcmfmo.html

stop)  echo "停止" ;;
来源：http://hz.gzhubu.top/gtitzontiy.html

*)     echo "未知命令" ;;
来源：http://hz.yongpay.top/gtalqoaipy.html

esac
来源：http://hz.guowangkeji.top/gtgezjdylv.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtpdcgbvbg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtfjabkhlp.html

[R13] for 计数循环
来源：http://hz.xuetiantiany.cn/gtwspmchsx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.52xcode.cn/gtllodftgs.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtepxhvgpd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtewhbkiuy.html

[R15] while 逐行读文件
来源：http://hz.hfpthk.cn/gtnheycxjc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yvedp.cn/gtvllyznfo.html

[R16] until 等待条件
来源：http://hz.zhongyouzk.top/gtlhsryibu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.52xcode.cn/gtjqkkxzef.html

[R17] 数组定义与取值
来源：http://hz.andypj.xyz/gtuihfairw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuetiantiany.cn/gtctidmrik.html

[R18] 遍历数组
来源：http://hz.feifeiyinyue.top/gtwxgbqnrs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cdnleiting.top/gtqqslwkyt.html

[R19] 数组长度
来源：http://hz.ydzc1.top/gtoymkymtw.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtdfohqudp.html

[R20] 关联数组（字典）
来源：http://hz.havefunace.top/gtvpgihuop.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.svipenyu.cn/gtdtvbguws.html

[R21] 字符串长度
来源：http://hz.wangdashe.top/gtiqmafren.html

echo "${#s}"
来源：http://hz.tianlin.xyz/gtugvhcfeb.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtnfbzgybm.html

echo "${s:0:5}"
来源：http://hz.haohaochexian.top/gtjuitprzz.html

[R23] 字符串替换
来源：http://hz.zdqjudy.top/gtjftpzgek.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhongyouzk.top/gtdhceryci.html

[R24] 大小写转换
来源：http://hz.aibaodan.cn/gtomsiasec.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yueranfly.top/gtjserqwfw.html

[R25] 去后缀 / 去前缀
来源：http://hz.hfpthk.cn/gthtzuxqfv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtkjliqigt.html

[R26] 命令替换
来源：http://hz.iojbl.cn/gtagofyuxo.html

now=$(date +%F); echo "$now"
来源：http://hz.hnqzz.top/gtjbjzdoru.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtokflarum.html

echo $((1 + 2 * 3))
来源：http://hz.0kj1m.cn/gtagzoxnad.html

[R28] 浮点运算
来源：http://hz.hnxiangtu.top/gtdiihippd.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhengqikj.top/gtoayuitlh.html

[R29] 定义函数
来源：http://hz.yangfankeji.com/gtlyfarjsp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xziqi.cn/gtiuzbpohf.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtdpudztir.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtgdljkmkx.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtuqvmtmsp.html

f() { local x=1; echo "$x"; }
来源：http://hz.dianchejie.cn/gtjrkyyjjw.html

[R32] 参数个数校验
来源：http://hz.cheryme.top/gtyrxoalvc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sysykeji.top/gtfhwdmzqj.html

[R33] 捕获错误并提示行号
来源：http://hz.smart0.xyz/gtzyjegqza.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuetiantiany.cn/gthiuhhtbk.html

[R34] 退出时清理
来源：http://hz.xinyue.icu/gtjcmclrhb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtuncnvtey.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtvogbwsnf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aibaodan.cn/gthsuzpsaa.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtugevorcd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.daxiang520.top/gtrftavsin.html

[R37] 把输出赋给变量
来源：http://hz.hnqzz.top/gtrytdfnes.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtnnufyehq.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtbaxzakpu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yanxiufei.cn/gtavewbpif.html

[R39] 重定向标准输出与错误
来源：http://hz.aizwys.cn/gtnwthqvod.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gttmpggals.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gtueujivjz.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtkreshuop.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtwklpzqay.html

cmd >/dev/null 2>&1
来源：http://hz.jiagoushi.top/gtllcaplpc.html

[R42] 输入重定向
来源：http://hz.jqgfzy.top/gtallkqbyy.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtmccxumnb.html

[R43] 按名字查找文件
来源：http://hz.bjfxy.top/gtqecarzcx.html

find . -name "*.log" -type f
来源：http://hz.snrcjt.cn/gtxpeaauwr.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtdqvgtrvj.html

find . -mtime -7 -type f
来源：http://hz.guowangkeji.top/gtqbcbdpfp.html

[R45] 批量删除
来源：http://hz.dashuyun.cn/gtnrcpzcqb.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtoedlblsv.html

[R46] 递归替换文件内容
来源：http://hz.snrcjt.cn/gtpqnzuigh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtvozdagar.html

[R47] sed 单行替换
来源：http://hz.meibo888.top/gtxfywzadf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnxiangtu.top/gtnkxwdynr.html

[R48] awk 取指定列
来源：http://hz.shuidangran.top/gtjlsanqhc.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtmjtyupug.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtbiakikpd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtbxixgdtr.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtpekmkuej.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gtrjwfggjj.html

[R51] 排序去重取前几
来源：http://hz.jinyuanbaomall.cn/gtptvxkkjf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.0kj1m.cn/gtubsebnyr.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtaoljqqgc.html

wc -l a.txt
来源：http://hz.xylfe.cn/gtyoeqlvvq.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtsimclawx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuanzx.com/gtswlvacrw.html

[R54] 比较两个文件
来源：http://hz.hysaishi.cn/gtjzgulhuf.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gtxqidrsyw.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtxbpuzozy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj202588.top/gtfsmrtkvi.html

[R56] 远程拷贝
来源：http://hz.jyoumei.cn/gtqcekgdpx.html

scp file user@host:/path/
来源：http://hz.tian-w.cn/gtdqpezbcl.html

[R57] 远程执行命令
来源：http://hz.haohaochexian.top/gtybaafuvt.html

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtzrpryphf.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtskimbspf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtxhdmtefh.html

[R59] 发 POST JSON
来源：http://hz.jqgufenzy.top/gtxeucogxw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gtxifypclz.html

[R60] 只看 HTTP 状态码
来源：http://hz.sufxvd.cn/gtgmfxulst.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtynarnxzy.html

[R61] 磁盘占用
来源：http://hz.ehwqpu.com/gtyfpwbnox.html

df -h;  du -sh *
来源：http://hz.mhx1999.top/gtelrddqlu.html

[R62] 找最占空间的文件
来源：http://hz.ehwqpu.com/gtjulcqovb.html

du -ah . | sort -rh | head -10
来源：http://hz.redwolf501.top/gtehqinvkn.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gtkltggkjd.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gthzbbwttb.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtgzgiajij.html

kill -9 $(pgrep -f app.py)
来源：http://hz.haohaochexian.top/gtrguqqakm.html

[R65] 查看端口占用
来源：http://hz.ivvv.top/gtuztremql.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.9152youxi.cn/gtpseaactw.html

[R66] 定时任务
来源：http://hz.wangdashe.top/gtrhzgrrmm.html

crontab -e;  crontab -l
来源：http://hz.hongshengwenyu.top/gtxhwirvsf.html

[R67] 生成随机十六进制串
来源：http://hz.dianchejie.cn/gtmugdmlby.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gtepmyjqvl.html

[R68] 计算文件校验值
来源：http://hz.jyoumei.cn/gtnorvbhve.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gtnlynlkln.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gtrllstepn.html

head -c 16 /dev/urandom | base64
来源：http://hz.xziqi.cn/gtdtqfwhxr.html

[R70] 时间戳与互转
来源：http://hz.feifeiyinyue.top/gtfedadfxa.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gthmyexgph.html

[R71] 日期格式化
来源：http://hz.nwbrower.top/gtgpldsmwx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtsdynrahi.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtakhoxevo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gtizxeumgv.html

[R73] 分割大日志
来源：http://hz.tianlin.xyz/gtwdnfmslc.html

split -l 1000 big.log part_
来源：http://hz.dashuyun.cn/gtryjqnprb.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gtzfspurdu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtgfykmzmc.html

[R75] 导出环境变量
来源：http://hz.yj20258.top/gtcfkuibvt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gttpcetyvn.html

[R76] 使用临时文件
来源：http://hz.chenzaomai.com/gtxcpsjwod.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtrdhlfdrq.html

[R77] 读取用户输入
来源：http://hz.xuanzx.com/gtctcasnly.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gtffxfoliz.html

[R78] 交互式菜单
来源：http://hz.yuanzhike.top/gtijiofeey.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtqiykybwl.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtjdvsuqng.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pengpengdd.cyou/gtgkzqucni.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtcicjplqi.html

time ./run.sh
来源：http://hz.xingfuxueyuan.xyz/gtogdgxgui.html

================================================================================
来源：http://hz.zhongyouzk.top/gtyopjnvfn.html

S. C / C++ 专题
来源：http://hz.jinyuanbaomall.cn/gtmuurkibt.html

================================================================================
来源：http://hz.zhongyouzk.top/gthfkydpov.html

[S01] C：Hello World
来源：http://hz.dianchejie.cn/gtppxgdqhf.html

#include <stdio.h>
来源：http://hz.redwolf501.top/gthfmmbcup.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aizwys.cn/gtizvvfgbf.html

[S02] C：变量与格式化输出
来源：http://hz.aizwys.cn/gtszoecgbh.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gtaredumse.html

[S03] C：读入整数
来源：http://hz.ybcxt.top/gtdgevamem.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gtkmpyeukh.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtggpsrawe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhaomingkeji.xyz/gtfwihgkum.html

[S05] C：字符串长度
来源：http://hz.hnqzz.top/gtpmnnvgxd.html

strlen(s)
来源：http://hz.chenzaomai.com/gtfoowxehn.html

[S06] C：字符串比较
来源：http://hz.zdqjudy.top/gtwaghfdkp.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gthjiqcbey.html

[S07] C：数组遍历求和
来源：http://hz.wangdashe.top/gtsrzncgtm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtrizvhocm.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gteptglvcv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtajphslvn.html

[S09] C：结构体定义与初始化
来源：http://hz.fengsongda.top/gtqjelcwdv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhoulong.xyz/gtizbvsskn.html

[S10] C：指针与解引用
来源：http://hz.yueranfly.top/gtshpdldwe.html

int *p = &a;  *p = 5;
来源：http://hz.chenzaomai.com/gtnzmkwdzr.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtthqmztxh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuanzx.com/gtpsotseqj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtthnflsyp.html

fclose(f);
来源：http://hz.zdqjudy.top/gtezzkzivz.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gttvbyyvbt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gtokwojcps.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtlmuswohu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.9152youxi.cn/gtpmdvuvdh.html

[S14] C：枚举
来源：http://hz.jinyuanbaomall.cn/gtqqbgksjo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gtzkhqbbyk.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtoiuwxjdd.html

(double) a / b
来源：http://hz.cqqwz.cn/gttljraexf.html

[S16] C：位操作置位
来源：http://hz.hongshengwenyu.top/gtrtvffgvb.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtdpppuzcx.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtloeexbee.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cheryme.top/gtnmrbnbjm.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gttenzagyv.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtmcyltvow.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gthnpdsjvn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtwowfnmbw.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtgignsukk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtetaieiwd.html

[S21] C：字符类别判断
来源：http://hz.cucudq.cn/gthmcmfppb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xinyue.icu/gtwqqcqhai.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gthlrexoxs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtvvfphpbx.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtvvsgdlfd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.quarkkingdee.top/gttefgzbvn.html

[S24] C：获取本地时间
来源：http://hz.sysykeji.top/gtxanxbwol.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtowpzmhkl.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtoeaovfwf.html

memcpy(dst, src, n);
来源：http://hz.wangdashe.top/gtmrykcriu.html

[S26] C：内存清零
来源：http://hz.ywan-chungtsiang.top/gtvqgoqjze.html

memset(a, 0, sizeof a);
来源：http://hz.daria6918.cn/gtfzvsglcw.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gthcsbbafh.html

const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtiatxkztr.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gtxazcudqt.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtpndgwumh.html

[S29] C：变参函数
来源：http://hz.c1oappe.top/gtqsmphrfl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtltnkclvq.html

[S30] C：头文件保护
来源：http://hz.fengsongda.top/gttnzwgcxf.html

#ifndef X_H
来源：http://hz.aizwys.cn/gtbudjyecd.html

#define X_H
来源：http://hz.ivvv.top/gtygvfizgy.html

#endif
来源：http://hz.ywan-chungtsiang.top/gtznfcqjib.html

[S31] C++：Hello World
来源：http://hz.zhengqikj.top/gtdcndapgu.html

#include <iostream>
来源：http://hz.yongpay.top/gtxiqyuvty.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtccutcfnl.html

[S32] C++：字符串
来源：http://hz.jinqigfzy.top/gthjwkznpo.html

std::string s = "hi";  s += "!";
来源：http://hz.c1oappe.top/gtxmmekfkv.html

[S33] C++：vector 增删
来源：http://hz.yueranfly.top/gtlbnbxkqm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guannengcc.top/gtwgdncpuo.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtcggbhlqa.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gteqhmhqeh.html

[S35] C++：map
来源：http://hz.ivvv.top/gtcuwrbkgq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtrbidrxhg.html

[S36] C++：unordered_map
来源：http://hz.fzhhl.top/gtueoeyiik.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtwfahjjwz.html

[S37] C++：set
来源：http://hz.316326.xyz/gtumqpdhcc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtiwehvznb.html

[S38] C++：排序
来源：http://hz.yuanzhike.top/gtsgcyspkt.html

std::sort(v.begin(), v.end());
来源：http://hz.cdnleiting.top/gtquzeosoc.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtwsuwxvil.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydjk.org.cn/gtxxqtdqwi.html

[S40] C++：查找元素
来源：http://hz.xziqi.cn/gtampavauc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hfpthk.cn/gtpwvofnve.html

[S41] C++：类与构造函数
来源：http://hz.daxiang520.top/gtbuncqpmt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinyuanbaomall.cn/gtannjqelr.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gtywsvzfxc.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258888.top/gtenvelslx.html

[S43] C++：智能指针
来源：http://hz.snrcjt.cn/gtzfwznjev.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtbqaivmhc.html

[S44] C++：引用传参
来源：http://hz.gogol.net.cn/gtxaoddujw.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtvfmtxeap.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtflvqkadz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgufenzy.top/gtkbpvviwh.html

[S46] C++：函数模板
来源：http://hz.zdqjudy.top/gtqufmnazy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigfzy.top/gtxthqftte.html


<!-- 参考信息 -->