代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.ywan-chungtsiang.top/gtxkrprlrg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gttjcjxsze.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuanzhike.top/gtlrmlcwac.html

[Q49] 更新单行
来源：http://hz.pengpengdd.cyou/gtkdvwwkng.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gttpjqlimb.html

[Q50] 批量更新
来源：http://hz.ywan-chungtsiang.top/gteioumbsk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtmafvjkfv.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtmzftyiko.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tianlin.xyz/gtdpcoqezz.html

[Q52] 删除指定行
来源：http://hz.jqgufenzy.top/gtijjcaqoj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuxming.cn/gtmyqpusqi.html

[Q53] 按条件删除
来源：http://hz.chenlongwang.top/gtidrkkmsg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xinyue.icu/gtdqeebxht.html

[Q54] 清空表
来源：http://hz.sweek.top/gtqkovwadl.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtjavvvqub.html

[Q55] 排名（并列占位）
来源：http://hz.chenjidiqi.icu/gthpuuagcs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.redwolf501.top/gtaavracbl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dianchejie.cn/gthqynyixt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shuidangran.top/gtwqlhbsvx.html

[Q57] 行号
来源：http://hz.jinyuanbaomall.cn/gtrzoizbxj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tian-w.cn/gtgzrwehaa.html

[Q58] 累计求和
来源：http://hz.shuidangran.top/gtyimvgbnh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.smart0.xyz/gthehqulyn.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtrsjmkpyi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtsieyssbo.html

[Q60] 取上一行 / 下一行
来源：http://hz.yanxiufei.cn/gtlnxmypnf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj202588.top/gtqkpgwtpr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtnaghnjuf.html

[Q61] 移动平均
来源：http://hz.yuanzhike.top/gtfhodttzj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jianghu66.top/gtfxwolzhi.html

[Q62] 分组占比
来源：http://hz.zhoulong.xyz/gttkqzicfh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtpshzqptw.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtljjqeket.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtskonncru.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gttwfpknmb.html

COMMIT;
来源：http://hz.sysykeji.top/gtwccesxsw.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtuxuvusdh.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gticiqijbi.html

[Q66] 行锁查询
来源：http://hz.jqgfzy.top/gtjmhfgdyy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ppjwa.cn/gtegroccuv.html

[Q67] 设置隔离级别
来源：http://hz.0kj1m.cn/gtspgzynxq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gttsihpknh.html

[Q68] 保存点
来源：http://hz.jlsjyb.cn/gtgcuqofmm.html

SAVEPOINT sp1;
来源：http://hz.xuetiantiany.cn/gtgkcaxtqq.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtodobecdz.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtrumjuwyl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtnrslpytm.html

[Q70] 更新统计信息
来源：http://hz.xylfe.cn/gtpclivlyr.html

ANALYZE TABLE users;
来源：http://hz.jinghuilouyu.cn/gtcjxttcvo.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gtguaturoj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gtesokamgm.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtntqtdpru.html

SHOW INDEX FROM users;
来源：http://hz.shanyushiyangtech.top/gtxeqbpvec.html

[Q73] 查看表状态
来源：http://hz.zhengqikj.top/gtdztktscu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhongyouzk.top/gtemsavojb.html

[Q74] 强制使用索引
来源：http://hz.yuanzhike.top/gtlwzzvoyi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aizwys.cn/gtjfznucta.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gtizvuzggf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cucudq.cn/gtqxnotrbq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtscahcdlo.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gtujipeqkh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtazejxmcj.html

[Q77] 时间加减
来源：http://hz.shuidangran.top/gtilosdjto.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.52xcode.cn/gtzaicjmpc.html

[Q78] 当前时间
来源：http://hz.cdnleiting.top/gtpvywhamo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.quarkkingdee.top/gtpfuvxoxf.html

[Q79] 字符串拼接
来源：http://hz.jianghu66.top/gtshjszqjq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hongshengwenyu.top/gtdzwrapss.html

[Q80] 字符串截取
来源：http://hz.jqgfzy.top/gtirikutgf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hfpthk.cn/gtifquxzba.html

[Q81] 字符串替换
来源：http://hz.tanke756.top/gtmxhutxxv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhengqikj.top/gtcwhgyobw.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtbhhfnipr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gticdnuwfg.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gthybrvldj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtyerkmqbl.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtddbdqpdp.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtdvinclet.html

[Q85] 数值取整
来源：http://hz.jqgfzy.top/gtahyxwxkt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenzaomai.com/gtgzxvxudx.html

[Q86] 读取 JSON 字段
来源：http://hz.meibo888.top/gtbhxytapz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ehwqpu.com/gtsxhudxsb.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gtpzhnxwkr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gtgdzxjtzj.html

[Q88] 行转列（条件聚合）
来源：http://hz.c1oappe.top/gttfoirhvv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtrtqoplzc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shangyingyoupin.top/gtqdlzipac.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gtscywjcih.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gzhubu.top/gttylohytx.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtkqyzofra.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pengpengdd.cyou/gtpvrzjqds.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqdvvygwj.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtlqlksvad.html

================================================================================
来源：http://hz.fzhhl.top/gtazxpmfys.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtkgzgczsd.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtuywgngok.html

set -euo pipefail
来源：http://hz.jqgufenzy.top/gtfnfljlwv.html

[R02] 变量赋值与使用
来源：http://hz.52xcode.cn/gtdhvqbgmg.html

name="Tom"; echo "$name"
来源：http://hz.xuetiantiany.cn/gtujrajiui.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtmpruktjg.html

readonly PI=3.14
来源：http://hz.hongshengwenyu.top/gtqevcizrm.html

[R04] 位置参数
来源：http://hz.shzxlz.cn/gtkedfvgef.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtfceezyov.html

[R05] 参数默认值
来源：http://hz.jinqigfzy.top/gtsixucjgt.html

name="${1:-default}"
来源：http://hz.ybcxt.top/gtmtdumxjn.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtonlcxanr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.meibo888.top/gthcqsdhnf.html

[R07] if 判断文件
来源：http://hz.nwbrower.top/gtztqtwmes.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nwbrower.top/gtgvmempjk.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtdoadawjd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.mhx1999.top/gtsppwfdkz.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gthcfgspqg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtckayofol.html

[R10] 正则匹配
来源：http://hz.yuanzhike.top/gtrfekloqt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gtyngwsjrw.html

[R11] case 多分支
来源：http://hz.hnqzz.top/gtflftwubq.html

case "$1" in
来源：http://hz.smart0.xyz/gtdxtdxfpd.html

start) echo "启动" ;;
来源：http://hz.quarkkingdee.top/gtvoqsktgc.html

stop)  echo "停止" ;;
来源：http://hz.dianchejie.cn/gtgehdduwh.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gteetsablr.html

esac
来源：http://hz.jiagoushi.top/gtoagekdgp.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtlyrcynlb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zdqjudy.top/gtzlnmkzpz.html

[R13] for 计数循环
来源：http://hz.zycfv.cn/gtunzjjxpk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xziqi.cn/gtqadgkeet.html

[R14] C 风格 for
来源：http://hz.hfpthk.cn/gtrpinypxe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hysaishi.cn/gtgmyirvxo.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtduvreuxp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tian-w.cn/gthwnqoeie.html

[R16] until 等待条件
来源：http://hz.yongpay.top/gtekhprscs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtycswhvyd.html

[R17] 数组定义与取值
来源：http://hz.chenlongwang.top/gtshetlpvr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ywan-chungtsiang.top/gthsrojzgv.html

[R18] 遍历数组
来源：http://hz.shzxlz.cn/gtepifvjrv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gtlbhautoa.html

[R19] 数组长度
来源：http://hz.zhoulong.xyz/gtasqfnmch.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtqtvyuwck.html

[R20] 关联数组（字典）
来源：http://hz.hywenlv.cn/gtcyilxgtr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gttezrzbbs.html

[R21] 字符串长度
来源：http://hz.jianghu66.top/gtmiplhfey.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtfmtshwyy.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtvcermtdl.html

echo "${s:0:5}"
来源：http://hz.cdnleiting.top/gtpckqqnlf.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtpfamkvwr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pengpengdd.cyou/gteezlikck.html

[R24] 大小写转换
来源：http://hz.meibo888.top/gtqdpbfklj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydjk.org.cn/gtmhgaqmhu.html

[R25] 去后缀 / 去前缀
来源：http://hz.guannengcc.top/gtovureelr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jianghu66.top/gtrpgzmirt.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtdniabsxs.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtdojptpmw.html

[R27] 算术展开
来源：http://hz.shanyushiyangtech.top/gtetwrriap.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gterbnojtv.html

[R28] 浮点运算
来源：http://hz.yangfankeji.com/gtluuheggn.html

echo "scale=2; 10/3" | bc
来源：http://hz.snrcjt.cn/gtxzralgfz.html

[R29] 定义函数
来源：http://hz.tianlin.xyz/gtnaqrqylh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yangfankeji.com/gtqhacquhh.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtcuzycitt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guowangkeji.top/gthusckbis.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtqnadrkzh.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gtybazgzhb.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtthzrlkpz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtaaieeypl.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtfwkgsnkl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ppjwa.cn/gtdyrgascw.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtgyprxvhk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtyaklbeuo.html

[R35] 后台执行并等待
来源：http://hz.yj20258888.top/gtgykltckb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shzxlz.cn/gtmuoppkzn.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gtmqmiqqfq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtrpocnjcn.html

[R37] 把输出赋给变量
来源：http://hz.ppjwa.cn/gtqzonvwkc.html

files=$(ls -1)
来源：http://hz.zhixingplan.top/gtkykrkqbo.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtpxlnzmvi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinyuanbaomall.cn/gtwpmtagmh.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gtnhvaefel.html

cmd > out.log 2>&1
来源：http://hz.zhengqikj.top/gtqxbhtbzy.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtttuqezfu.html

echo "log" >> out.log
来源：http://hz.svipenyu.cn/gtqeluukux.html

[R41] 丢弃输出
来源：http://hz.andypj.xyz/gtwajzfygq.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtjqtmqxgk.html

[R42] 输入重定向
来源：http://hz.dashuyun.cn/gterswjgns.html

wc -l < a.txt
来源：http://hz.shuidangran.top/gtpvudwkse.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gtmcnkxsko.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtdruvybim.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtizmhjagb.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gtjxivoamr.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtssynirfp.html

find . -name "*.tmp" -delete
来源：http://hz.zhijiandao.cn/gtiugmdgox.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtvcztkynj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ivvv.top/gtxwrowlhc.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtqhturkdn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sweek.top/gtzqeahnor.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtkguuyelu.html

awk '{print $1, $3}' a.txt
来源：http://hz.cdnleiting.top/gtiuqlcdxc.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtkwrrbexo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtukmyyamt.html

[R50] awk 求和
来源：http://hz.xingfuxueyuan.xyz/gtiknbgjbe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtneomikvv.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gthzignwba.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xylfe.cn/gtzeuuoxgq.html

[R52] 统计行数
来源：http://hz.wangshuangyany.cn/gtavbtzthc.html

wc -l a.txt
来源：http://hz.wangdashe.top/gtdufqxmxo.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtmkdqeieh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtujkbdahc.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtlhiviufv.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtrxwnmkzm.html

[R55] 压缩与解压
来源：http://hz.dashuyun.cn/gtojondhcf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jiagoushi.top/gtolahhmmn.html

[R56] 远程拷贝
来源：http://hz.cdnleiting.top/gttuyzxqcc.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtgpnptbgl.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtaazsmgst.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtxjxbjtbe.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtsfqrhxwk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtpamkdyme.html

[R59] 发 POST JSON
来源：http://hz.nanxinkj.top/gtiiuuyepm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pycfn.com/gtvfiqnxqb.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtarodpwfk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jiagoushi.top/gtpwqirjuw.html

[R61] 磁盘占用
来源：http://hz.hammf.cn/gtvcnuonfo.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtmydzkzhw.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtcxvaurie.html

du -ah . | sort -rh | head -10
来源：http://hz.guowangkeji.top/gtwalkribt.html

[R63] 内存与进程
来源：http://hz.bjfxy.top/gtlalxcixs.html

free -h;  ps aux | grep nginx
来源：http://hz.chenzaomai.com/gtcgudbwes.html

[R64] 结束进程
来源：http://hz.bjfxy.top/gtiqchrxig.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtoxgxxjfq.html

[R65] 查看端口占用
来源：http://hz.jiagoushi.top/gtmiadvxwa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuxming.cn/gtlxhnvqxs.html

[R66] 定时任务
来源：http://hz.dashuyun.cn/gttujfbuzi.html

crontab -e;  crontab -l
来源：http://hz.iojbl.cn/gtfkulfbsg.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtpivyaaiw.html

openssl rand -hex 16
来源：http://hz.jinqigufen.top/gtotonfnsf.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtuidkgdtj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtjuceotod.html

[R69] 生成随机密码
来源：http://hz.aibaodan.cn/gtzuwyweii.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtqqpfgrgx.html

[R70] 时间戳与互转
来源：http://hz.gogol.net.cn/gteylxrgyf.html

date +%s;  date -d @1700000000
来源：http://hz.yuanzhike.top/gtkacdrvpu.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gthoqkzase.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.vqdsnc.cn/gtpardkmly.html

[R72] 等待端口就绪
来源：http://hz.cashguo.top/gthsmkmbhk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hywenlv.cn/gtnwukokss.html

[R73] 分割大日志
来源：http://hz.zycfv.cn/gthxllqluj.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gtohnxgynd.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gtghmfwemr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xylfe.cn/gtbcirtgbi.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtducljypj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pycfn.com/gtlgszgbuj.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtafvltwsp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtfqxkoqcu.html

[R77] 读取用户输入
来源：http://hz.zhaomingkeji.xyz/gtgtgjxrit.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtglgsqqgd.html

[R78] 交互式菜单
来源：http://hz.gaohongyu789.top/gtlrwsgzti.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ivvv.top/gthaecgwmh.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gtznzbyvrw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cucudq.cn/gthfevfbxe.html

[R80] 查看脚本执行耗时
来源：http://hz.birdmap.top/gtbumgtfkm.html

time ./run.sh
来源：http://hz.yangfankeji.com/gtkhcqiwtx.html

================================================================================
来源：http://hz.yanxiufei.cn/gtlsjwazsu.html

S. C / C++ 专题
来源：http://hz.yueranfly.top/gtzuzszkxa.html

================================================================================
来源：http://hz.guannengcc.top/gtzhsrapqw.html

[S01] C：Hello World
来源：http://hz.svipenyu.cn/gtizopnteo.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtlfxsjqvf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hfpthk.cn/gtzknaboep.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtkhmybmtv.html

int a = 10; printf("%d\n", a);
来源：http://hz.tianlin.xyz/gtlflnkuif.html

[S03] C：读入整数
来源：http://hz.dashuyun.cn/gtdrsqtwoc.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gttbborewe.html

[S04] C：字符串复制
来源：http://hz.bjfxy.top/gtzfyoatsn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtsvajmegx.html

[S05] C：字符串长度
来源：http://hz.ppjwa.cn/gtkztvzmmx.html

strlen(s)
来源：http://hz.guannengcc.top/gtmpbnzyzq.html

[S06] C：字符串比较
来源：http://hz.pycfn.com/gtraqdmhry.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtylkeigme.html

[S07] C：数组遍历求和
来源：http://hz.ehwqpu.com/gtzcmwcgnl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ehwqpu.com/gtkzwrxtkk.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtwxhqtmkh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtzbwfxmty.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtznzyoqro.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydzc1.top/gtfnhmwloh.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtxcvmmjur.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtmwjkiagz.html

[S11] C：逐行读文件
来源：http://hz.gaohongyu789.top/gtmkjggqsu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtyzarfrri.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.haohaochexian.top/gtodesfpmn.html

fclose(f);
来源：http://hz.cdnleiting.top/gtvfhjmzul.html

[S12] C：写文件
来源：http://hz.gzhubu.top/gtaiokhkuh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtlupznihc.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtnylvreof.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xingfuxueyuan.xyz/gtkaponmgn.html

[S14] C：枚举
来源：http://hz.tian-w.cn/gtrkmpmjac.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.redwolf501.top/gthpidrywg.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gtpgapvdvi.html

(double) a / b
来源：http://hz.ydjk.org.cn/gtimonupmx.html

[S16] C：位操作置位
来源：http://hz.sweek.top/gtogyckrre.html

x |= (1 << 3);
来源：http://hz.yj202588.top/gtlxgeclcb.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtbvxaegzm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gthidpsddq.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gttaopwnix.html


<!-- 参考信息 -->