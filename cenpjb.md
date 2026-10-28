代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gtotjobxaa.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtrqanbnzn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cdnleiting.top/gtpsjxzvqw.html

[Q74] 强制使用索引
来源：http://hz.zhongyouzk.top/gtkoscpchz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gaohongyu789.top/gtwxjvwfya.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gthblrmrma.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtisvibsvf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhijiandao.cn/gtqzlllmfs.html

[Q76] 按天统计
来源：http://hz.shanyushiyangtech.top/gtcemnjwsb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangshuangyany.cn/gtqqihhbar.html

[Q77] 时间加减
来源：http://hz.redwolf501.top/gtaewjwosi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuetiantiany.cn/gtrsvtvlyq.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gtxrkbjusd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhixingplan.top/gtrhkjoprg.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtwpohxueo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sxryk.cn/gtunwdrsnm.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtzvlmfvcn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtvmcbgoom.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtujmypmya.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cucudq.cn/gthqpljxvk.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtjqcjzkuk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydzc1.top/gtzpxvwzvw.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gttdfvxnlh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtvcgnjckc.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtqctgdwyi.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigfzy.top/gtiaqagaax.html

[Q85] 数值取整
来源：http://hz.dashuyun.cn/gtqhjpdrmq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtejcjoxrq.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtawcrdlxd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guannengcc.top/gtexjojgsu.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gtkhearqse.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cashguo.top/gtlhmkxiop.html

[Q88] 行转列（条件聚合）
来源：http://hz.guannengcc.top/gtowzaxqom.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtyufwcwht.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guannengcc.top/gtgoahqevf.html

[Q89] 判断表是否存在
来源：http://hz.cheryme.top/gttdnzldkx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj202588.top/gtrvpyrkhs.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtqybbdyxf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258888.top/gtlzubykua.html

================================================================================
来源：http://hz.dianchejie.cn/gttzkognrk.html

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtmsuyqfii.html

================================================================================
来源：http://hz.shzxlz.cn/gtmvqefyqs.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtsuhxvorp.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtavxlqkqy.html

set -euo pipefail
来源：http://hz.xziqi.cn/gtuxxgxwru.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtamojxcir.html

name="Tom"; echo "$name"
来源：http://hz.ehwqpu.com/gtrbllyvcn.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtlhqztlft.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gtxexmpdgo.html

[R04] 位置参数
来源：http://hz.daria6918.cn/gtkxoqpert.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yvedp.cn/gtsvrxeyez.html

[R05] 参数默认值
来源：http://hz.yueranfly.top/gtqsrtygqi.html

name="${1:-default}"
来源：http://hz.ehwqpu.com/gtfrzwygpx.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtalcbamlz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sweek.top/gtqxsbltdm.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gtxydgngxz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gthnoaymly.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gttjskoupy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtrkcxotwc.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtpuvjelqs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gtkrnbmwmc.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtbhutfjkv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhongyouzk.top/gtursgxcxn.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtqblifuqe.html

case "$1" in
来源：http://hz.yuxming.cn/gtjkujaqec.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gttkxnztcz.html

stop)  echo "停止" ;;
来源：http://hz.sufxvd.cn/gtkdoocvcy.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtteuishnb.html

esac
来源：http://hz.yvedp.cn/gtfgwqsllp.html

[R12] for 遍历文件
来源：http://hz.xziqi.cn/gtjrpocbhl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtozneafqf.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtogdjmhky.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gthkawocvn.html

[R14] C 风格 for
来源：http://hz.ivvv.top/gtyfutjskh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gtcbkrhofj.html

[R15] while 逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gthokvrivn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gthbglsaxf.html

[R16] until 等待条件
来源：http://hz.zdqjudy.top/gtfxzbclbv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtjdllrgik.html

[R17] 数组定义与取值
来源：http://hz.jiagoushi.top/gtzaxfqlie.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtxdkpotli.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gtmithxdqe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aibaodan.cn/gtjbrjeici.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtwpguaure.html

echo "${#arr[@]}"
来源：http://hz.jinghuilouyu.cn/gtjxtzznad.html

[R20] 关联数组（字典）
来源：http://hz.ybcxt.top/gtfjeahkkp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cqqwz.cn/gtkzppbiti.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gttnznmngl.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtzhqbmepj.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtzslndnzn.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtdlerthxk.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtqfdxdobd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuanzx.com/gtegwrzpum.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gttmzermch.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yuxming.cn/gtrqqdzklj.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhiwuduotai.top/gteqegjuth.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangkeji.top/gtprthlluc.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtryrxbemq.html

now=$(date +%F); echo "$now"
来源：http://hz.316326.xyz/gtawsniklj.html

[R27] 算术展开
来源：http://hz.yueranfly.top/gtssgzanno.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gtsxfdhrny.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtpwlcbhkh.html

echo "scale=2; 10/3" | bc
来源：http://hz.jianghu66.top/gtgsoluqal.html

[R29] 定义函数
来源：http://hz.tianlin.xyz/gtcxbjqjrw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhaomingkeji.xyz/gtcarzcsfp.html

[R30] 函数返回状态码
来源：http://hz.ywan-chungtsiang.top/gtantbvxiy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daria6918.cn/gtmhstydlw.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtvekrvcls.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtefgqmgal.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gtabgzebvs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtxdkicgjx.html

[R33] 捕获错误并提示行号
来源：http://hz.iojbl.cn/gtkdeaghul.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guannengcc.top/gtsencuieg.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtmfygncke.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtfodxiybm.html

[R35] 后台执行并等待
来源：http://hz.zhiwuduotai.top/gtrgladhuo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigufen.top/gtzogcxgft.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtlcjebozi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gthnoldrgp.html

[R37] 把输出赋给变量
来源：http://hz.ppjwa.cn/gtapjbwice.html

files=$(ls -1)
来源：http://hz.ydzc1.top/gtocaqseop.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtxbnjfevg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtraupnjyw.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtfvndwwzc.html

cmd > out.log 2>&1
来源：http://hz.xuetiantiany.cn/gtvfnjsyzt.html

[R40] 追加写日志
来源：http://hz.havefunace.top/gtlwqdjthv.html

echo "log" >> out.log
来源：http://hz.jinqigfzy.top/gtvcwpeabx.html

[R41] 丢弃输出
来源：http://hz.xziqi.cn/gtecomvvlk.html

cmd >/dev/null 2>&1
来源：http://hz.fzhhl.top/gtgyoctxji.html

[R42] 输入重定向
来源：http://hz.jiagoushi.top/gtbdzoeezd.html

wc -l < a.txt
来源：http://hz.guowangkeji.top/gtwbwwaufx.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gttujfmfdk.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtcebndtab.html

[R44] 按修改时间查找
来源：http://hz.jinyuanbaomall.cn/gtdxrwjarb.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtcnbqpzhn.html

[R45] 批量删除
来源：http://hz.gzhubu.top/gtkltcnnlp.html

find . -name "*.tmp" -delete
来源：http://hz.yanxiufei.cn/gthaptrqbh.html

[R46] 递归替换文件内容
来源：http://hz.sxryk.cn/gtnrdhpxun.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nwbrower.top/gtznjgeiqk.html

[R47] sed 单行替换
来源：http://hz.jyoumei.cn/gtgxuulcgt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aizwys.cn/gtahyqwpwg.html

[R48] awk 取指定列
来源：http://hz.ppjwa.cn/gtvkzwqbkd.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhongyouzk.top/gtrckbpbst.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtpfoqehwy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtmcrvnanc.html

[R50] awk 求和
来源：http://hz.zhoulong.xyz/gtsmynyesv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangshuangyany.cn/gtlmtqxmlw.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gthnjawxzf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhaomingkeji.xyz/gtkpdjmpqb.html

[R52] 统计行数
来源：http://hz.smart0.xyz/gtbzgbfsdu.html

wc -l a.txt
来源：http://hz.sysykeji.top/gtrhtolgew.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtgccsjctg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tanke756.top/gtljlggosg.html

[R54] 比较两个文件
来源：http://hz.jyoumei.cn/gtpacckwqx.html

diff a.txt b.txt
来源：http://hz.hfpthk.cn/gturbzjgbs.html

[R55] 压缩与解压
来源：http://hz.nanxuanxn.top/gtqyvjlrud.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cdnleiting.top/gtijasgmsj.html

[R56] 远程拷贝
来源：http://hz.aizwys.cn/gtxjrmyura.html

scp file user@host:/path/
来源：http://hz.meibo888.top/gtabosvnil.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtdfkmnvyp.html

ssh user@host 'uptime'
来源：http://hz.sysykeji.top/gtrpqhovvn.html

[R58] 下载文件
来源：http://hz.xziqi.cn/gtawcaldwh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.kuanghao11.cn/gtyfxyrxuu.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtjtgxtjju.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtjcolhxed.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtoirvtdkq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtmjfebont.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtlwziuacv.html

df -h;  du -sh *
来源：http://hz.zhongyouzk.top/gtjeooqgvg.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtikuwvjol.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtbrxwzdjd.html

[R63] 内存与进程
来源：http://hz.316326.xyz/gtxcxuktwo.html

free -h;  ps aux | grep nginx
来源：http://hz.jiagoushi.top/gtwexbnxto.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gttnvrgolg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jiagoushi.top/gtpxjsoles.html

[R65] 查看端口占用
来源：http://hz.ydzc1.top/gtqryerikc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtxhxgoepz.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtgakhfzlw.html

crontab -e;  crontab -l
来源：http://hz.xinyue.icu/gtiflczvwu.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gtfaenwolz.html

openssl rand -hex 16
来源：http://hz.gzhubu.top/gtjpucdxtw.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gthrcsrxcc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.mhx1999.top/gtrnsijzzu.html

[R69] 生成随机密码
来源：http://hz.fengsongda.top/gtctrraven.html

head -c 16 /dev/urandom | base64
来源：http://hz.cheryme.top/gtqraaiyly.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtnsquvtbz.html

date +%s;  date -d @1700000000
来源：http://hz.shuidangran.top/gtzbxsdzjx.html

[R71] 日期格式化
来源：http://hz.zhengqikj.top/gtnjvugwng.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtrhjmxovv.html

[R72] 等待端口就绪
来源：http://hz.ehwqpu.com/gtpswscjed.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj202588.top/gtfhldylim.html

[R73] 分割大日志
来源：http://hz.wangshuangyany.cn/gtgeyspapn.html

split -l 1000 big.log part_
来源：http://hz.jianghu66.top/gtzmlzhdky.html

[R74] 批量重命名
来源：http://hz.aibaodan.cn/gtixlrxldh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gtouzxfsza.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gthjrusaaj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtecokcsvs.html

[R76] 使用临时文件
来源：http://hz.aizwys.cn/gtcjuvedfd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtpppwzens.html

[R77] 读取用户输入
来源：http://hz.zhongyouzk.top/gthdtxmyxc.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtjpjdxfls.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtrbvqcbnt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gthvrkmrcr.html

[R79] 解析命令行选项
来源：http://hz.kuanghao11.cn/gtmyplwgsn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtlbwjzvtt.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gtpzttvvjg.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtrlvbvwol.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfmkrjvyx.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gteoeskknp.html

================================================================================
来源：http://hz.0kj1m.cn/gtxfxbsphq.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gtcusrxtfs.html

#include <stdio.h>
来源：http://hz.kuanghao11.cn/gtsfazfmhi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sysykeji.top/gtrzfgkdyy.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtywsyjhbn.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gtzaoiclyw.html

[S03] C：读入整数
来源：http://hz.zhaomingkeji.xyz/gtosvpiita.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtiiecrrep.html

[S04] C：字符串复制
来源：http://hz.shzxlz.cn/gtevfjpiev.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtyvaxrtng.html

[S05] C：字符串长度
来源：http://hz.cucudq.cn/gtkeehqzer.html

strlen(s)
来源：http://hz.shanyushiyangkeji.top/gtanmwjrtj.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gttompcqjh.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gtqbfytsnn.html

[S07] C：数组遍历求和
来源：http://hz.daria6918.cn/gtzdpzawev.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangkeji.top/gttiwptxjc.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtrnwhtccx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gtrivynxnf.html

[S09] C：结构体定义与初始化
来源：http://hz.ivvv.top/gtwnvxffrx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258.top/gtsrxqyfnl.html

[S10] C：指针与解引用
来源：http://hz.iojbl.cn/gtlkfyoaqu.html

int *p = &a;  *p = 5;
来源：http://hz.cheryme.top/gtdspjqrgq.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtvfrjiyto.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtqpcoeosb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yvedp.cn/gtomjuipzs.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtqllpbcdx.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtrxzycfiv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtpnhlxtge.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtfbcdittq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtlrgrgbfv.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtfvohypex.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtqtfcczok.html

[S15] C：类型转换
来源：http://hz.chenjidiqi.icu/gtgeapapqy.html

(double) a / b
来源：http://hz.ydjk.org.cn/gtppjaxirb.html

[S16] C：位操作置位
来源：http://hz.zhengqikj.top/gtuutmtxku.html

x |= (1 << 3);
来源：http://hz.tanke756.top/gtmbbljlxl.html

[S17] C：安全拼接字符串
来源：http://hz.zhixingplan.top/gtgoidnsdm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtqrjsylfa.html

[S18] C：命令行参数
来源：http://hz.316326.xyz/gtgtwxynzn.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtyrbdryvr.html

[S19] C：快速排序
来源：http://hz.zhongyouzk.top/gtrxmbnqrh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtoonlzdjt.html

[S20] C：二分查找
来源：http://hz.jianghu66.top/gtsvmnfpuf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtcbwulbrw.html

[S21] C：字符类别判断
来源：http://hz.zhengqikj.top/gtqgtxzxbl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dianchejie.cn/gtbzdnjfws.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtlukdwswc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangshuangyany.cn/gtypdxkwsk.html

[S23] C：随机数
来源：http://hz.jinyuanbaomall.cn/gtjgzzypvi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dashuyun.cn/gtklgennih.html

[S24] C：获取本地时间
来源：http://hz.meibo888.top/gtoeoygvfn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgufenzy.top/gtrmkfnkgr.html

[S25] C：内存拷贝
来源：http://hz.yuanzhike.top/gttdbtnhfz.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtubrjmjsf.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtvsqfvkhb.html

memset(a, 0, sizeof a);
来源：http://hz.wangshuangyany.cn/gtmaawfahd.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gthafzbfii.html

const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtmhnlndfg.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtfstxjiqh.html

static int counter = 0;
来源：http://hz.smart0.xyz/gtghexpoko.html

[S29] C：变参函数
来源：http://hz.sysykeji.top/gtrnrtdrro.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gtjnsatpnu.html

[S30] C：头文件保护
来源：http://hz.jianghu66.top/gtjsjpjzjm.html

#ifndef X_H
来源：http://hz.316326.xyz/gtqwthpvig.html

#define X_H
来源：http://hz.tanke756.top/gtalrlyake.html

#endif
来源：http://hz.vqdsnc.cn/gtazdjjbhv.html

[S31] C++：Hello World
来源：http://hz.tianlin.xyz/gtvmctihlw.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gtdhosopzf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.svipenyu.cn/gttddizgjo.html

[S32] C++：字符串
来源：http://hz.chenzaomai.com/gtjxgabvns.html

std::string s = "hi";  s += "!";
来源：http://hz.sysykeji.top/gttlljpqoc.html

[S33] C++：vector 增删
来源：http://hz.havefunace.top/gtdpwjyumf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtgbaukzjl.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtekrotdqh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258888.top/gtwaaulizp.html

[S35] C++：map
来源：http://hz.yj202588.top/gtpenyxixn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtfelaukte.html

[S36] C++：unordered_map
来源：http://hz.jiagoushi.top/gtjttrtmkv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtoqyhckiq.html

[S37] C++：set
来源：http://hz.yvedp.cn/gtewfuvkdg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtxkfwaluz.html

[S38] C++：排序
来源：http://hz.iojbl.cn/gtquspjqno.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gtdaorptyh.html

[S39] C++：自定义比较器排序
来源：http://hz.daxiang520.top/gtipwmzlui.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgufenzy.top/gtgeozrscx.html

[S40] C++：查找元素
来源：http://hz.hywenlv.cn/gttydjhqix.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtnevyhpzj.html

[S41] C++：类与构造函数
来源：http://hz.nwbrower.top/gtouqfvggd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gtxlxkyoxv.html

[S42] C++：继承与虚函数
来源：http://hz.chenlongwang.top/gtryymsmwz.html

class B : public Base { public: void f() override {} };
来源：http://hz.vqdsnc.cn/gtbegdsoun.html


<!-- 参考信息 -->