代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gthadlwwgd.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gtnfcnllsz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gtwbhlmqxi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhaomingkeji.xyz/gtathhzaio.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtdwsdjfhm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnqzz.top/gtsqvcuodo.html

[Q77] 时间加减
来源：http://hz.fengsongda.top/gtjnfzaxfb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gotoacloud.top/gtdleomagh.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gtjttbowdo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gtnngegbpo.html

[Q79] 字符串拼接
来源：http://hz.chenzaomai.com/gtzpmxqrmt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yonumen.top/gteyfatiur.html

[Q80] 字符串截取
来源：http://hz.jlsjyb.cn/gtbuizkoog.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenjidiqi.icu/gtbabzttwi.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtdrngaoaz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tian-w.cn/gtenpdsmot.html

[Q82] 字符长度与字节长度
来源：http://hz.yvedp.cn/gtlpjxdsvo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cdnleiting.top/gthowychsf.html

[Q83] 大小写转换
来源：http://hz.shangyingyoupin.top/gtzfxwnehj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtkqxtyffm.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gtnicrjfiu.html

SELECT TRIM(name) FROM users;
来源：http://hz.smart0.xyz/gtfgbvyfcp.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtweybsupi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhengqikj.top/gtsmbyzzwz.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gtjxprrdyo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.snrcjt.cn/gtcdauytul.html

[Q87] JSON 字段做条件
来源：http://hz.yueranfly.top/gtpivigkdf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhongyouzk.top/gtkaiaswan.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtegetzkdo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hywenlv.cn/gtltcqtkes.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangshuangyany.cn/gtqnfgruwl.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtrnxvizqy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtltjrfovz.html

[Q90] 生成序号列
来源：http://hz.hywenlv.cn/gtcfkfhepf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aibaodan.cn/gtdhnyvsgs.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttibyehyz.html

R. Bash 专题
来源：http://hz.chenjidiqi.icu/gtvnfhjyas.html

================================================================================
来源：http://hz.daria6918.cn/gtypkejlrk.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gtnkvuzuuu.html

#!/usr/bin/env bash
来源：http://hz.yangfankeji.com/gtxiwezltr.html

set -euo pipefail
来源：http://hz.nanxinkj.top/gtmgifovaz.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtbqfkxzxt.html

name="Tom"; echo "$name"
来源：http://hz.xylfe.cn/gtmzayrrzw.html

[R03] 只读变量
来源：http://hz.cheryme.top/gtygfdxpfv.html

readonly PI=3.14
来源：http://hz.hammf.cn/gtnhosjvpt.html

[R04] 位置参数
来源：http://hz.316326.xyz/gtimoxbqol.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtogxkkipw.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtqrbpzqen.html

name="${1:-default}"
来源：http://hz.feifeiyinyue.top/gtidekgkmu.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangtech.top/gtnkirrrnf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtrjixwqgt.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gtokcfinav.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xziqi.cn/gtahvcaqag.html

[R08] 数值比较
来源：http://hz.zhaomingkeji.xyz/gtokmlwadk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xinyue.icu/gtttlnonbz.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gtnuyqvvmw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtqcbcwkmy.html

[R10] 正则匹配
来源：http://hz.jinqigfzy.top/gtrgtrymzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhoulong.xyz/gtzkcurtma.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtmocjeabd.html

case "$1" in
来源：http://hz.yonumen.top/gtmmbfaivq.html

start) echo "启动" ;;
来源：http://hz.chenlongwang.top/gtsgccjbgh.html

stop)  echo "停止" ;;
来源：http://hz.xuanzx.com/gtiswlojux.html

*)     echo "未知命令" ;;
来源：http://hz.jyoumei.cn/gtexgsrzhr.html

esac
来源：http://hz.jinyuanbaomall.cn/gthprmmnmz.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gtvcvrtupb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtyxdwxqev.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtkfgebhhz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gtwudpyocf.html

[R14] C 风格 for
来源：http://hz.yj20258.top/gtxblbsjoj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtpesmfipi.html

[R15] while 逐行读文件
来源：http://hz.yonumen.top/gtegdmclft.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cqqwz.cn/gteidlsnei.html

[R16] until 等待条件
来源：http://hz.cheryme.top/gttqeruvxj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnqzz.top/gtkbebkkuq.html

[R17] 数组定义与取值
来源：http://hz.hongshengwenyu.top/gtmwbikadx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtqsbtuacm.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gtkpujmlcl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtgqsteyar.html

[R19] 数组长度
来源：http://hz.daxiang520.top/gtritribnb.html

echo "${#arr[@]}"
来源：http://hz.gzhubu.top/gtmzcrzitp.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gtmgkpurya.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xingfuxueyuan.xyz/gtvitqcjxj.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtsnagutfx.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtokhhawoe.html

[R22] 截取子串
来源：http://hz.wangshuangyany.cn/gtqveclosa.html

echo "${s:0:5}"
来源：http://hz.sufxvd.cn/gtoxemwxcd.html

[R23] 字符串替换
来源：http://hz.chenjidiqi.icu/gtrnehxmzl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtzgbsjpcr.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtmjkorutr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtlrutnpdr.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhixingplan.top/gthqzrfhpz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cucudq.cn/gtxpzncrfr.html

[R26] 命令替换
来源：http://hz.hysaishi.cn/gtlfpubomd.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtisxgvfmz.html

[R27] 算术展开
来源：http://hz.yonumen.top/gtuotylyyb.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtorfloscd.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gteenjvndk.html

echo "scale=2; 10/3" | bc
来源：http://hz.nwbrower.top/gtmxwlfmku.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtqufovfzy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.9152youxi.cn/gtmulxpxou.html

[R30] 函数返回状态码
来源：http://hz.meibo888.top/gtvdyjxccl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtmwxuahht.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtsbkfrycm.html

f() { local x=1; echo "$x"; }
来源：http://hz.jlsjyb.cn/gtsbxfukzy.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangtech.top/gtxjzijwsv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtypfgjqcy.html

[R33] 捕获错误并提示行号
来源：http://hz.zhoulong.xyz/gtpuwjndcg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinyuanbaomall.cn/gtoexxzqan.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtebjtilzz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtuqkmjabn.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtmtxiosxn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.c1oappe.top/gtlytpalyo.html

[R36] 并发执行多个任务
来源：http://hz.xziqi.cn/gtbjiihjhh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtfvfngqrr.html

[R37] 把输出赋给变量
来源：http://hz.zhengqikj.top/gtadzzzgwb.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtgwazomvt.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtjoyaorhs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhixingplan.top/gtqhhjtogy.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gttlcjfgsp.html

cmd > out.log 2>&1
来源：http://hz.hammf.cn/gtwqarffco.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtkmofllex.html

echo "log" >> out.log
来源：http://hz.guannengcc.top/gteuxuooqy.html

[R41] 丢弃输出
来源：http://hz.wangshuangyany.cn/gtdhzdiynx.html

cmd >/dev/null 2>&1
来源：http://hz.zhoulong.xyz/gtxxsrfujo.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gtrmgtdpmb.html

wc -l < a.txt
来源：http://hz.xingfuxueyuan.xyz/gtxzwasoxg.html

[R43] 按名字查找文件
来源：http://hz.zycfv.cn/gthqnwlgyd.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtoxkgljnz.html

[R44] 按修改时间查找
来源：http://hz.9152youxi.cn/gtywztyxus.html

find . -mtime -7 -type f
来源：http://hz.andypj.xyz/gtnopywbmh.html

[R45] 批量删除
来源：http://hz.birdmap.top/gtitvhowxz.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtyboqctnr.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtimlybkya.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hammf.cn/gtjajydqyd.html

[R47] sed 单行替换
来源：http://hz.redwolf501.top/gtdzmwkrzf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gttycbhnae.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtegvaggsv.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtjwamnoeb.html

[R49] awk 带条件
来源：http://hz.meibo888.top/gtgbqgxinr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtqhtfuzyy.html

[R50] awk 求和
来源：http://hz.havefunace.top/gtnzamesto.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtmxjvvjyp.html

[R51] 排序去重取前几
来源：http://hz.cqqwz.cn/gtqnjicmuy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtoemghkck.html

[R52] 统计行数
来源：http://hz.havefunace.top/gtccuxxqgi.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gttiyndomc.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtdbtspxjq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.mhx1999.top/gtehybwhgd.html

[R54] 比较两个文件
来源：http://hz.cdnleiting.top/gtiqhwxoqj.html

diff a.txt b.txt
来源：http://hz.quarkkingdee.top/gtysfpydfp.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtypmczlfx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.0kj1m.cn/gtnmvwpufn.html

[R56] 远程拷贝
来源：http://hz.zycfv.cn/gtplwdncjk.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtnocjazdy.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gttkgmgjgq.html

ssh user@host 'uptime'
来源：http://hz.tanke756.top/gtmjgleknw.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gticfvkmwo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xinyue.icu/gtdtheylzq.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtzvotwssf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtfajrfbpv.html

[R60] 只看 HTTP 状态码
来源：http://hz.yueranfly.top/gtsbyjvytn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtnmonthsc.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtmlzmjksd.html

df -h;  du -sh *
来源：http://hz.fzhhl.top/gtkrpokrdk.html

[R62] 找最占空间的文件
来源：http://hz.feifeiyinyue.top/gtqylpczhe.html

du -ah . | sort -rh | head -10
来源：http://hz.hnxiangtu.top/gtufgrladz.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtceisoqzx.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gtdzjgorzx.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtikbxhppg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xinyue.icu/gtwwteoiwq.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtqwqggasz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangkeji.top/gtsetrmwqf.html

[R66] 定时任务
来源：http://hz.yangfankeji.com/gtfqtglcyg.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gtehdcsdvm.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gtozruufdd.html

openssl rand -hex 16
来源：http://hz.gogol.net.cn/gteozmkofg.html

[R68] 计算文件校验值
来源：http://hz.zycfv.cn/gtmzpeffkm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gaohongyu789.top/gtkpyyawix.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gtiukatxpn.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtemohctto.html

[R70] 时间戳与互转
来源：http://hz.andypj.xyz/gtjicuobzs.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gthngewhfe.html

[R71] 日期格式化
来源：http://hz.sweek.top/gtguknevfy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gtrmwcnwnh.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtwuwkqxvg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.0kj1m.cn/gtfoijclmf.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtptyjcbxu.html

split -l 1000 big.log part_
来源：http://hz.cqqwz.cn/gtydhhwooq.html

[R74] 批量重命名
来源：http://hz.cheryme.top/gtpnkdlqzt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuanzx.com/gtnddqavxo.html

[R75] 导出环境变量
来源：http://hz.sweek.top/gtbawwigdg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gthcjpvqqw.html

[R76] 使用临时文件
来源：http://hz.chenlongwang.top/gtbsdhgcwe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtbwpepswp.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtajhqfpbo.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtlvgyqmbx.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtikdpvlxc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yvedp.cn/gtjoqvzmha.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtwyxzowks.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cdnleiting.top/gtvnrcpunk.html

[R80] 查看脚本执行耗时
来源：http://hz.xinyue.icu/gtyjkdcfml.html

time ./run.sh
来源：http://hz.daxiang520.top/gtjehyugrs.html

================================================================================
来源：http://hz.xylfe.cn/gtrelcvsbr.html

S. C / C++ 专题
来源：http://hz.nanxuanxn.top/gtcbvfyxkq.html

================================================================================
来源：http://hz.c1oappe.top/gtqoubpkfv.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gtelmihwrq.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtadbwseay.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtbpjlmyub.html

[S02] C：变量与格式化输出
来源：http://hz.bjfxy.top/gtqtogrkmu.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gtvqfekfny.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtbwsnbqhh.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gthcukypaj.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtwxladkvt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtievprlzw.html

[S05] C：字符串长度
来源：http://hz.xingfuxueyuan.xyz/gttgwguahe.html

strlen(s)
来源：http://hz.yvedp.cn/gtyyqjbucx.html

[S06] C：字符串比较
来源：http://hz.cheryme.top/gtefkacdnh.html

strcmp(a, b) == 0
来源：http://hz.guowangkeji.top/gtdmnsqytl.html

[S07] C：数组遍历求和
来源：http://hz.shuidangran.top/gtqzqqjfcc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tianlin.xyz/gtduaxwsqf.html

[S08] C：动态内存分配与释放
来源：http://hz.tanke756.top/gtojsnmbvb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cqqwz.cn/gtuwfojpcc.html

[S09] C：结构体定义与初始化
来源：http://hz.xuanzx.com/gtnrmpxvbv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jyoumei.cn/gtxhkpkkyp.html

[S10] C：指针与解引用
来源：http://hz.jianghu66.top/gtrypngyai.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtiuxrezmv.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gtdpfuuzlf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cheryme.top/gtorbazkmc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pycfn.com/gthtjvclwi.html

fclose(f);
来源：http://hz.sxryk.cn/gtnrbooacj.html

[S12] C：写文件
来源：http://hz.yj20258888.top/gtzybahbit.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtadwsfdnu.html

[S13] C：宏定义
来源：http://hz.ivvv.top/gtzqvkkoyv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aizwys.cn/gtpzdtpapf.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtlyrujpou.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtndnqqfar.html

[S15] C：类型转换
来源：http://hz.ydzc1.top/gtwljzelnf.html

(double) a / b
来源：http://hz.wangdashe.top/gtezoxdtiu.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtkswtnvig.html

x |= (1 << 3);
来源：http://hz.dianchejie.cn/gtewpkjktc.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtfkqgsqoh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jiagoushi.top/gtijxgmtws.html

[S18] C：命令行参数
来源：http://hz.gzhubu.top/gtqghqytmu.html

int main(int argc, char **argv)
来源：http://hz.jinqigfzy.top/gtvigemciu.html

[S19] C：快速排序
来源：http://hz.fzhhl.top/gtywftdcei.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtdcdoagpi.html

[S20] C：二分查找
来源：http://hz.shanyushiyangkeji.top/gttctljrjt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydzc1.top/gtfzhxhnzj.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gtrnvmifhk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hnxiangtu.top/gtzafqhioj.html

[S22] C：字符串转数字
来源：http://hz.wangdashe.top/gtfcsyrxlu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtluuaaylr.html

[S23] C：随机数
来源：http://hz.ehwqpu.com/gtppetdtrs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dashuyun.cn/gtsoisscep.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtjkykldsq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtyirsnewh.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtvzevykts.html

memcpy(dst, src, n);
来源：http://hz.shuidangran.top/gtzdqpgzsr.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtsbrgzuif.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigufen.top/gtjmylnpvq.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtwpvfwdvp.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtmxkuvkvi.html

[S28] C：静态变量
来源：http://hz.hywenlv.cn/gtsibujnwy.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtqeleikak.html

[S29] C：变参函数
来源：http://hz.cdnleiting.top/gtovoimobd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shzxlz.cn/gttedbdjqn.html

[S30] C：头文件保护
来源：http://hz.jinyuanbaomall.cn/gtopzimoyb.html

#ifndef X_H
来源：http://hz.ivvv.top/gthasjobam.html

#define X_H
来源：http://hz.feifeiyinyue.top/gtispiyyug.html

#endif
来源：http://hz.yuanzhike.top/gtrkedobux.html

[S31] C++：Hello World
来源：http://hz.hnxiangtu.top/gtikmxamho.html

#include <iostream>
来源：http://hz.hfpthk.cn/gtzhpowuji.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtlbpburgg.html

[S32] C++：字符串
来源：http://hz.316326.xyz/gtswoablqm.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxuanxn.top/gttnnmpsaa.html

[S33] C++：vector 增删
来源：http://hz.wangshuangyany.cn/gtoffeqrlh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.c1oappe.top/gtpoxesfzx.html

[S34] C++：遍历 vector
来源：http://hz.jyoumei.cn/gtshlgtxmx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtgctktxmr.html

[S35] C++：map
来源：http://hz.havefunace.top/gtxgcozkmy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtjgxexich.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gtinydiqfa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtqftlzesg.html

[S37] C++：set
来源：http://hz.aibaodan.cn/gtfbmsoeie.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtywlsqygv.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gtpcburtxr.html

std::sort(v.begin(), v.end());
来源：http://hz.tanke756.top/gtyoqfyjut.html

[S39] C++：自定义比较器排序
来源：http://hz.svipenyu.cn/gtazkqxbzi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xinyue.icu/gtwytxwngt.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gtqyxazlrj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtjrolklmg.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gtssiyylvr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtjfaozsbv.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtxlecybev.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gttupnorht.html

[S43] C++：智能指针
来源：http://hz.sufxvd.cn/gtfmososqx.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhiwuduotai.top/gtbfrpbudg.html

[S44] C++：引用传参
来源：http://hz.yuxming.cn/gtjvxtlosq.html

void inc(int &x) { ++x; }
来源：http://hz.yanxiufei.cn/gthzvkscuy.html


<!-- 参考信息 -->