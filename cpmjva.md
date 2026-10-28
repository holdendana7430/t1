代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtrdkacbqf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangshuangyany.cn/gtioitgqpm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtffmxkenv.html

[Q49] 更新单行
来源：http://hz.wangdashe.top/gtdjyncqnu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gthmnizdti.html

[Q50] 批量更新
来源：http://hz.hnxiangtu.top/gtrgfkpqba.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258888.top/gtdtaddqpn.html

[Q51] 用子查询更新
来源：http://hz.xinyue.icu/gtcvwcjbsk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xinyue.icu/gtvdhwcczg.html

[Q52] 删除指定行
来源：http://hz.yueranfly.top/gtqzwywdxg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ehwqpu.com/gtsbkfbojh.html

[Q53] 按条件删除
来源：http://hz.yonumen.top/gtjaqfphqt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gtphuggxvn.html

[Q54] 清空表
来源：http://hz.dashuyun.cn/gtuzwqxbof.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtgiinhpph.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangkeji.top/gtunkfwqtg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtkfqairkw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.316326.xyz/gtgzolhymp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtxysqsfzv.html

[Q57] 行号
来源：http://hz.haohaochexian.top/gtkvatjpuc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtcfbonhch.html

[Q58] 累计求和
来源：http://hz.ybcxt.top/gtffszjvxp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtrrfrbkiu.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtxayqzuei.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtqzoltsui.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtdxbwsbpx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtwsognwzc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtdphnkxdc.html

[Q61] 移动平均
来源：http://hz.nanxinkj.top/gtcghrxlzz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gtloijtqvl.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gtnppldpeo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtrvvrziix.html

[Q63] 开启事务
来源：http://hz.gotoacloud.top/gtklzmkjse.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yongpay.top/gtpvrxyjxn.html

[Q64] 提交事务
来源：http://hz.gogol.net.cn/gtdvwermfl.html

COMMIT;
来源：http://hz.xziqi.cn/gtputlfgwv.html

[Q65] 回滚事务
来源：http://hz.andypj.xyz/gtuxnmobdr.html

ROLLBACK;
来源：http://hz.zhoulong.xyz/gtuvozxdxo.html

[Q66] 行锁查询
来源：http://hz.yj202588.top/gtxxaeijwx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gttohzzqvg.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gtmagbwbzb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtliumraqw.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtcgilmigb.html

SAVEPOINT sp1;
来源：http://hz.xziqi.cn/gtbomtetqe.html

ROLLBACK TO sp1;
来源：http://hz.tianlin.xyz/gtwzfaetpc.html

[Q69] 查看执行计划
来源：http://hz.yj202588.top/gtoeaxbaxg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zdqjudy.top/gtjdlspfqh.html

[Q70] 更新统计信息
来源：http://hz.shzxlz.cn/gtsypqvowq.html

ANALYZE TABLE users;
来源：http://hz.pycfn.com/gtihunumht.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtsbslyeye.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuanzhike.top/gtblzehisj.html

[Q72] 查看索引
来源：http://hz.yueranfly.top/gtwkpcnywy.html

SHOW INDEX FROM users;
来源：http://hz.hysaishi.cn/gtesbrmzki.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtpvqotazn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhixingplan.top/gtyalgmdcl.html

[Q74] 强制使用索引
来源：http://hz.mhx1999.top/gttcvhobvv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhaomingkeji.xyz/gtdbjhcafx.html

[Q75] 日期格式化
来源：http://hz.ywan-chungtsiang.top/gtlngpxqsn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtdlvzcddw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shzxlz.cn/gtnpnnqehw.html

[Q76] 按天统计
来源：http://hz.ywan-chungtsiang.top/gtsvxfardg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxinkj.top/gtcmndwknz.html

[Q77] 时间加减
来源：http://hz.kuanghao11.cn/gtzkivbppi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dianchejie.cn/gtnvmsiynl.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gturjuwlje.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtrgxbfrrr.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gtkbcvrnka.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sufxvd.cn/gtveazwvtq.html

[Q80] 字符串截取
来源：http://hz.andypj.xyz/gtgqwdjrik.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sxryk.cn/gtpotvckhl.html

[Q81] 字符串替换
来源：http://hz.tian-w.cn/gtivaejzct.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhijiandao.cn/gtiwsdbfvs.html

[Q82] 字符长度与字节长度
来源：http://hz.zhengqikj.top/gtwmlkones.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtprassjoa.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtyjwkgpql.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj202588.top/gtrqvuzail.html

[Q84] 去除首尾空格
来源：http://hz.zhijiandao.cn/gttcapelep.html

SELECT TRIM(name) FROM users;
来源：http://hz.gogol.net.cn/gtchzrbaib.html

[Q85] 数值取整
来源：http://hz.cdnleiting.top/gtepvshfgw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtfcjuituj.html

[Q86] 读取 JSON 字段
来源：http://hz.daria6918.cn/gtmcpyaqcb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guowangkeji.top/gtpujadsty.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtjwrwyjyz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daria6918.cn/gtkgnfjeko.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtreborwhk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gthblwhjom.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtatqqfibi.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtwdoqwpur.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtauktsjhe.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtnoxfvcon.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yangfankeji.com/gtptecvmzd.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxwcyucdt.html

R. Bash 专题
来源：http://hz.sweek.top/gtucwfnonf.html

================================================================================
来源：http://hz.gogol.net.cn/gtgkmjqhia.html

[R01] shebang 与严格模式
来源：http://hz.aizwys.cn/gthkcpbmcz.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtmdnsxcfc.html

set -euo pipefail
来源：http://hz.gzhubu.top/gteauptqzj.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtmndcepsn.html

name="Tom"; echo "$name"
来源：http://hz.guannengcc.top/gtcvcqtuwa.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtddvixdqh.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gttnczufie.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtyrcgwemn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gotoacloud.top/gtozpujrqe.html

[R05] 参数默认值
来源：http://hz.sweek.top/gtwriqxtbb.html

name="${1:-default}"
来源：http://hz.zhoulong.xyz/gtlwsgnfwr.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtzekzuqdj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xylfe.cn/gtdnsvikql.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtxpyyusek.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtrjucgamx.html

[R08] 数值比较
来源：http://hz.jqgfzy.top/gtauxoobsm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.redwolf501.top/gtqywpguvx.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gtgqlsklzu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gtdksxzhsa.html

[R10] 正则匹配
来源：http://hz.jinghuilouyu.cn/gtgsrcjpah.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtfzyhedmx.html

[R11] case 多分支
来源：http://hz.pycfn.com/gtvdvamsam.html

case "$1" in
来源：http://hz.haohaochexian.top/gtzouofzgk.html

start) echo "启动" ;;
来源：http://hz.yangfankeji.com/gtrgahxoxk.html

stop)  echo "停止" ;;
来源：http://hz.316326.xyz/gtnzqpxeeb.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtsobjddsi.html

esac
来源：http://hz.sxryk.cn/gtfbbyxglh.html

[R12] for 遍历文件
来源：http://hz.zhaomingkeji.xyz/gthwhwibwb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhongyouzk.top/gtachuykxp.html

[R13] for 计数循环
来源：http://hz.tian-w.cn/gtbqpmuhhe.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtiuacujrh.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtwxopxask.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gthyhlrnmu.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtberdkhve.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinghuilouyu.cn/gtszluxmik.html

[R16] until 等待条件
来源：http://hz.xziqi.cn/gtxpvwwaao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtxogiggey.html

[R17] 数组定义与取值
来源：http://hz.chenzaomai.com/gtjovnysni.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnxiangtu.top/gtieplwmzf.html

[R18] 遍历数组
来源：http://hz.guannengcc.top/gtrdqkiyix.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gtytuvweiu.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtyrphcjgn.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtdsppxotn.html

[R20] 关联数组（字典）
来源：http://hz.yangfankeji.com/gteaaamybd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.snrcjt.cn/gtiyzarllz.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gthuarropm.html

echo "${#s}"
来源：http://hz.meibo888.top/gtsitunpnx.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtdyxdqrpb.html

echo "${s:0:5}"
来源：http://hz.yonumen.top/gthzhjwyhv.html

[R23] 字符串替换
来源：http://hz.fengsongda.top/gtovioudxd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinyuanbaomall.cn/gtvcmymzso.html

[R24] 大小写转换
来源：http://hz.pycfn.com/gtgxggzbqg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.9152youxi.cn/gtkzjgctgn.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtzdlghkil.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtjgwzvdmp.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtpnzmegdr.html

now=$(date +%F); echo "$now"
来源：http://hz.aibaodan.cn/gtksadpuwy.html

[R27] 算术展开
来源：http://hz.zhixingplan.top/gtpspxclhu.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtgicwffdu.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtwqqucopi.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtkqnbieiw.html

[R29] 定义函数
来源：http://hz.hysaishi.cn/gtwfaczctb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daria6918.cn/gtprplbxqk.html

[R30] 函数返回状态码
来源：http://hz.ivvv.top/gtrgfefctf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxuanxn.top/gtloykuyuq.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtxreiopog.html

f() { local x=1; echo "$x"; }
来源：http://hz.yonumen.top/gtfbhfyboc.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtrctxodga.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtnvwvwrar.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtqqfeqooc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtnofvwzvb.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtpcpoxbaz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtmkypiazc.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtgmhymrxq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.svipenyu.cn/gtnotuwson.html

[R36] 并发执行多个任务
来源：http://hz.nwbrower.top/gtyhioafsm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gaohongyu789.top/gtwowyxgdm.html

[R37] 把输出赋给变量
来源：http://hz.smart0.xyz/gtjogwbgib.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtqhtpyqli.html

[R38] 管道串联
来源：http://hz.zhengqikj.top/gtijqktvjt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtxebiitrv.html

[R39] 重定向标准输出与错误
来源：http://hz.jiagoushi.top/gtbxlhudpw.html

cmd > out.log 2>&1
来源：http://hz.xuetiantiany.cn/gtouzvtuhm.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtnyiezodi.html

echo "log" >> out.log
来源：http://hz.xuetiantiany.cn/gtixknstef.html

[R41] 丢弃输出
来源：http://hz.yueranfly.top/gtfucmdhrx.html

cmd >/dev/null 2>&1
来源：http://hz.smart0.xyz/gtwxvlmikk.html

[R42] 输入重定向
来源：http://hz.hnxiangtu.top/gtcyvagxci.html

wc -l < a.txt
来源：http://hz.hywenlv.cn/gtljxcgres.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtowaxziqg.html

find . -name "*.log" -type f
来源：http://hz.dianchejie.cn/gthclkcuew.html

[R44] 按修改时间查找
来源：http://hz.jiagoushi.top/gthwenovmr.html

find . -mtime -7 -type f
来源：http://hz.havefunace.top/gtbeuabxzz.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtipgygacp.html

find . -name "*.tmp" -delete
来源：http://hz.jqgfzy.top/gteadhyfdr.html

[R46] 递归替换文件内容
来源：http://hz.tianlin.xyz/gtouzonxaz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gttjyrvvqp.html

[R47] sed 单行替换
来源：http://hz.yj202588.top/gtyytyktrb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtejkartvt.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtggpxgnqs.html

awk '{print $1, $3}' a.txt
来源：http://hz.hywenlv.cn/gtkswgjina.html

[R49] awk 带条件
来源：http://hz.redwolf501.top/gtckrafqdg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gthzhkeuaw.html

[R50] awk 求和
来源：http://hz.nwbrower.top/gtuqnhqpgq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dashuyun.cn/gtvqzqpwro.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtybkxzqzm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ppjwa.cn/gtpyylqhcw.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtavmnguxg.html

wc -l a.txt
来源：http://hz.hammf.cn/gtkbviymxp.html

[R53] 查看文件头与实时尾
来源：http://hz.hywenlv.cn/gtwyfwoegf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtbbyailon.html

[R54] 比较两个文件
来源：http://hz.zhengqikj.top/gtjqjflhig.html

diff a.txt b.txt
来源：http://hz.daxiang520.top/gtqbdfchmv.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtaighzhba.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtsljdocqh.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtunrkchdk.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtiltpzyxh.html

[R57] 远程执行命令
来源：http://hz.nanxuanxn.top/gtsitxsprs.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtyxgpnafm.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtlnvqithp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangtech.top/gtdfshuien.html

[R59] 发 POST JSON
来源：http://hz.cashguo.top/gtiebenggx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtsompofmz.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtldjirono.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtluigkrqg.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtcnmqpoye.html

df -h;  du -sh *
来源：http://hz.jqgufenzy.top/gtzmmycjar.html

[R62] 找最占空间的文件
来源：http://hz.gogol.net.cn/gtazhcveuv.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtswwhmeda.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtotttapix.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtrwpyfkmy.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtucejoqwq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtgqzpuyzf.html

[R65] 查看端口占用
来源：http://hz.bjfxy.top/gtwtkeshvj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtyxoygyvj.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtsrqtnwdc.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtlzepgpke.html

[R67] 生成随机十六进制串
来源：http://hz.chenlongwang.top/gtklaxcyxt.html

openssl rand -hex 16
来源：http://hz.redwolf501.top/gthbhrlqwo.html

[R68] 计算文件校验值
来源：http://hz.nanxinkj.top/gtqiwfnvqw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtbcvfilir.html

[R69] 生成随机密码
来源：http://hz.aibaodan.cn/gtwtfaihsg.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtruewbdnu.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtnxbgbcro.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtuwpmpheg.html

[R71] 日期格式化
来源：http://hz.xziqi.cn/gtdenqplyo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aibaodan.cn/gtsctoyjox.html

[R72] 等待端口就绪
来源：http://hz.ybcxt.top/gtizjuqvhw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtyjrwfhjl.html

[R73] 分割大日志
来源：http://hz.jinyuanbaomall.cn/gtvkeuzsch.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gtmxpndycr.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gttaqeorjf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.svipenyu.cn/gtwwypekum.html

[R75] 导出环境变量
来源：http://hz.zycfv.cn/gtkubryfhc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gtdaqwfeeq.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtiteeizym.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtkdoljgjl.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gttilpcxmh.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gtgsaiqobj.html

[R78] 交互式菜单
来源：http://hz.yvedp.cn/gtewmkxpvs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtwyakaepy.html

[R79] 解析命令行选项
来源：http://hz.hywenlv.cn/gtwfarqhwo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zdqjudy.top/gtpczlugye.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtfukhsbxr.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtuzidwfjz.html

================================================================================
来源：http://hz.nanxinkj.top/gtllbbdbzu.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtmbjlexpj.html

================================================================================
来源：http://hz.jinqigufen.top/gtxwcscael.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gtbpyfvtpi.html

#include <stdio.h>
来源：http://hz.xinyue.icu/gtdhvlstji.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtzwawnyyq.html

[S02] C：变量与格式化输出
来源：http://hz.chenjidiqi.icu/gtecrehgrf.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gtxiqvujcb.html

[S03] C：读入整数
来源：http://hz.yj202588.top/gtzmpxchoq.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtgsqogjpq.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gthhaibxuj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtfmlrzlhc.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gtrxexcbyu.html

strlen(s)
来源：http://hz.hywenlv.cn/gtvahpprgq.html

[S06] C：字符串比较
来源：http://hz.0kj1m.cn/gteawyiljv.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtpcawoqwj.html

[S07] C：数组遍历求和
来源：http://hz.9152youxi.cn/gtdchelrhm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtqwqrplef.html

[S08] C：动态内存分配与释放
来源：http://hz.hongshengwenyu.top/gtmvvecbzg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dianchejie.cn/gtmkdvxvhu.html

[S09] C：结构体定义与初始化
来源：http://hz.gotoacloud.top/gtltsopayg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yongpay.top/gtvxxoajak.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gtuylrlvwn.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangtech.top/gtslaqctca.html

[S11] C：逐行读文件
来源：http://hz.haohaochexian.top/gtnrjkusbd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zycfv.cn/gteeosgjti.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtivwkaqdf.html

fclose(f);
来源：http://hz.tian-w.cn/gtsfbslqqk.html

[S12] C：写文件
来源：http://hz.shzxlz.cn/gtbchyvoaz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gtwbavxuye.html

[S13] C：宏定义
来源：http://hz.hammf.cn/gtvlgjsjgj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtgrvbxmdz.html

[S14] C：枚举
来源：http://hz.yj202588.top/gtbbjuioda.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtcnruihiy.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtdkjomqyy.html

(double) a / b
来源：http://hz.guannengcc.top/gtvyaqjqtt.html

[S16] C：位操作置位
来源：http://hz.yj20258.top/gtmynvamyj.html

x |= (1 << 3);
来源：http://hz.yj20258888.top/gtyzmuaszf.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gteecljpiz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtypuioorw.html

[S18] C：命令行参数
来源：http://hz.jiagoushi.top/gteeglzidv.html


<!-- 参考信息 -->