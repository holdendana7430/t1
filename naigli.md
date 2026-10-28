代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.gzhubu.top/gtbvtvoqhz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ehwqpu.com/gtbagskmpx.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtvqqauaia.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gttxoljfyh.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtfnceuuom.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xylfe.cn/gtwsgfbgre.html

[Q45] EXISTS 判断存在
来源：http://hz.0kj1m.cn/gtjexcjhgm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtctzamnbs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnqzz.top/gtakgkkzog.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtcwmbzpvs.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gtyhxxlvla.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sxryk.cn/gtbwdqfjlz.html

[Q48] CTE 公用表表达式
来源：http://hz.ybcxt.top/gtxxyxnmjg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xylfe.cn/gtmfpzjkpy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.mhx1999.top/gtuzijhpya.html

[Q49] 更新单行
来源：http://hz.yvedp.cn/gtvjrdbxtu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gtkwycgaoz.html

[Q50] 批量更新
来源：http://hz.jiagoushi.top/gtwsyinluo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtnhzkujxn.html

[Q51] 用子查询更新
来源：http://hz.chenzaomai.com/gtfmzoghco.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtenrouwqk.html

[Q52] 删除指定行
来源：http://hz.cdnleiting.top/gtcyyjtacy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sxryk.cn/gttldketxj.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtupudqgrx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.smart0.xyz/gtnjsqichq.html

[Q54] 清空表
来源：http://hz.zycfv.cn/gtavnwhfwx.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtzbkffzae.html

[Q55] 排名（并列占位）
来源：http://hz.zycfv.cn/gtgzpduqsj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sweek.top/gtwcxsxpaa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gthfklcpcr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dianchejie.cn/gthgebwnth.html

[Q57] 行号
来源：http://hz.jinghuilouyu.cn/gtmxishohl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yangfankeji.com/gttzpruamb.html

[Q58] 累计求和
来源：http://hz.shanyushiyangtech.top/gtjkehoydp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gogol.net.cn/gtymnarhtl.html

[Q59] 分组内累计
来源：http://hz.wangshuangyany.cn/gtmndsxiri.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtzwvxkmmw.html

[Q60] 取上一行 / 下一行
来源：http://hz.jyoumei.cn/gtbwmeqhlu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.9152youxi.cn/gtrdjhyhuz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtihugoakp.html

[Q61] 移动平均
来源：http://hz.nwbrower.top/gtoxkafxan.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ehwqpu.com/gtjpknshds.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtmjyjkyhw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtcmlcobyf.html

[Q63] 开启事务
来源：http://hz.xziqi.cn/gtmjjqlpla.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuanzx.com/gtwwapwbzy.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtmwiopmqx.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtumxtppck.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gthwvzmpkh.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtehgzdrqs.html

[Q66] 行锁查询
来源：http://hz.yueranfly.top/gtbiqlgrgo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnqzz.top/gtwgmfbagl.html

[Q67] 设置隔离级别
来源：http://hz.tianlin.xyz/gtgutrhqah.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gzhubu.top/gtpgtitilc.html

[Q68] 保存点
来源：http://hz.quarkkingdee.top/gtqrbuyfbd.html

SAVEPOINT sp1;
来源：http://hz.xylfe.cn/gtcnoewkfe.html

ROLLBACK TO sp1;
来源：http://hz.meibo888.top/gtikaxapca.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtzbgdjiso.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fzhhl.top/gtdhhjmfho.html

[Q70] 更新统计信息
来源：http://hz.chenjidiqi.icu/gtjradkkmd.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtndrcdzyl.html

[Q71] 查看建表语句
来源：http://hz.kuanghao11.cn/gtpnaavxav.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fengsongda.top/gtkrqwuglu.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtqdspcpfu.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtspyteckw.html

[Q73] 查看表状态
来源：http://hz.dashuyun.cn/gtwokmufgx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hysaishi.cn/gtwvetuhfc.html

[Q74] 强制使用索引
来源：http://hz.xingfuxueyuan.xyz/gtnwkbsxvy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.9152youxi.cn/gtjbapqked.html

[Q75] 日期格式化
来源：http://hz.redwolf501.top/gtpwuhdpfo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yanxiufei.cn/gtrtbcvrlq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shzxlz.cn/gtsbrkwztr.html

[Q76] 按天统计
来源：http://hz.cashguo.top/gtsckiywtc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtryctsvtw.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtypcvcshr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtsyfudcpc.html

[Q78] 当前时间
来源：http://hz.aibaodan.cn/gtvpllutey.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yongpay.top/gtziowlgxl.html

[Q79] 字符串拼接
来源：http://hz.guowangkeji.top/gtgonvcadw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhoulong.xyz/gtjuxviqcu.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtkslujkhk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.birdmap.top/gtupkoaizx.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangtech.top/gtxrrzppgz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.smart0.xyz/gtumfohhxc.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtwiallbhl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gthceeuswr.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtskaydrdq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dashuyun.cn/gtubrdtzah.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtkdgptnsx.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258888.top/gtfxsfwalt.html

[Q85] 数值取整
来源：http://hz.snrcjt.cn/gtqbueodry.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.meibo888.top/gteudmsbuz.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtiegbnplr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hysaishi.cn/gtnkasejju.html

[Q87] JSON 字段做条件
来源：http://hz.gzhubu.top/gtmptcppho.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shzxlz.cn/gtdwuyhevh.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtatbvzdpq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.havefunace.top/gtomhoppnf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.svipenyu.cn/gtwdkkmism.html

[Q89] 判断表是否存在
来源：http://hz.guannengcc.top/gtmfivhyap.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gttejfdpye.html

[Q90] 生成序号列
来源：http://hz.xingfuxueyuan.xyz/gtttvxyeul.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.52xcode.cn/gtgesflzlx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtsgrtsljy.html

R. Bash 专题
来源：http://hz.hfpthk.cn/gtkonlgpqd.html

================================================================================
来源：http://hz.guannengcc.top/gtfmzygwdg.html

[R01] shebang 与严格模式
来源：http://hz.sxryk.cn/gtnkovizsd.html

#!/usr/bin/env bash
来源：http://hz.pycfn.com/gtgyupnxfo.html

set -euo pipefail
来源：http://hz.birdmap.top/gtxosiwbvy.html

[R02] 变量赋值与使用
来源：http://hz.sxryk.cn/gttntslcto.html

name="Tom"; echo "$name"
来源：http://hz.jlsjyb.cn/gtmiznuqyw.html

[R03] 只读变量
来源：http://hz.guowangkeji.top/gtpcxyccpd.html

readonly PI=3.14
来源：http://hz.zhoulong.xyz/gtegrkiisx.html

[R04] 位置参数
来源：http://hz.bjfxy.top/gtmkywypcw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhiwuduotai.top/gtxxkndnkb.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtxvzpxbvw.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gttkpqwcfs.html

[R06] 判断命令是否存在
来源：http://hz.shzxlz.cn/gtvaboljna.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.birdmap.top/gtkepvcewy.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtgbwrtkhm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.feifeiyinyue.top/gtjnzcxmsx.html

[R08] 数值比较
来源：http://hz.aibaodan.cn/gtzffwmwbd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.birdmap.top/gtgfcclyin.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtuxyxydvv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.c1oappe.top/gtjghbinra.html

[R10] 正则匹配
来源：http://hz.yj202588.top/gtvgwfxwuz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtssrlvzns.html

[R11] case 多分支
来源：http://hz.shuidangran.top/gtezrtvxhs.html

case "$1" in
来源：http://hz.meibo888.top/gtjhicjsql.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtqrrqzqpx.html

stop)  echo "停止" ;;
来源：http://hz.zdqjudy.top/gtxmrpvdzv.html

*)     echo "未知命令" ;;
来源：http://hz.xinyue.icu/gtllsqwgyy.html

esac
来源：http://hz.smart0.xyz/gtxeriqzxd.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtnojoxxmm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.quarkkingdee.top/gtpatssnva.html

[R13] for 计数循环
来源：http://hz.mhx1999.top/gtywuptoqa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jlsjyb.cn/gthjwuyubz.html

[R14] C 风格 for
来源：http://hz.yuxming.cn/gtlamxehbj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtxeiqwrhz.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gttgqpztlz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.316326.xyz/gtlmrxkouj.html

[R16] until 等待条件
来源：http://hz.gaohongyu789.top/gtcbfogemj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtqabwymzs.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtgidhkscb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtmxpwrbzs.html

[R18] 遍历数组
来源：http://hz.meibo888.top/gtmzxenvih.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258.top/gtrgzauzdr.html

[R19] 数组长度
来源：http://hz.vqdsnc.cn/gtriktcbyt.html

echo "${#arr[@]}"
来源：http://hz.c1oappe.top/gtdupvddum.html

[R20] 关联数组（字典）
来源：http://hz.zhijiandao.cn/gtfkljlhlt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shzxlz.cn/gtkakjbcjg.html

[R21] 字符串长度
来源：http://hz.yj20258.top/gtpencdain.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtyziwcmxg.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtdrqvmoua.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gteyrpqdvu.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gtpcrkdybk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pengpengdd.cyou/gtnedavewy.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtaxgkwsgy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gaohongyu789.top/gtstiaqjbe.html

[R25] 去后缀 / 去前缀
来源：http://hz.jlsjyb.cn/gtvkmafdjy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gthjnnrnhr.html

[R26] 命令替换
来源：http://hz.havefunace.top/gtahnomonr.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtdiadvsxl.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtvmqzjaqu.html

echo $((1 + 2 * 3))
来源：http://hz.ivvv.top/gtvyjorkwr.html

[R28] 浮点运算
来源：http://hz.ydjk.org.cn/gtfaannbeb.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gttrsozuiu.html

[R29] 定义函数
来源：http://hz.shangyingyoupin.top/gtnqomlaac.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258.top/gtjijxsbxc.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtlhkkpcnm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gtsbywchst.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtkukcqcrh.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtxrymmysj.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtokpofope.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj202588.top/gtwbwzvbau.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258.top/gttcaksadc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hywenlv.cn/gtlvcfeauq.html

[R34] 退出时清理
来源：http://hz.hammf.cn/gtcanvbfmc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtkxsdrstp.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtvdpkglvy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.9152youxi.cn/gtfgvuwcdn.html

[R36] 并发执行多个任务
来源：http://hz.jqgufenzy.top/gtvhxymunx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yanxiufei.cn/gtnkptqwpf.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gtfffxqdbk.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtzkbmuben.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtirsosyal.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhijiandao.cn/gtdaeabcjw.html

[R39] 重定向标准输出与错误
来源：http://hz.havefunace.top/gtrqdmhwdp.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtqdslmhxq.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtqpywifhv.html

echo "log" >> out.log
来源：http://hz.guowangkeji.top/gtssjmkcwl.html

[R41] 丢弃输出
来源：http://hz.9152youxi.cn/gthugxmzyo.html

cmd >/dev/null 2>&1
来源：http://hz.cqqwz.cn/gtlaaclkpf.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtngtwriwj.html

wc -l < a.txt
来源：http://hz.fzhhl.top/gtfbapydmv.html

[R43] 按名字查找文件
来源：http://hz.yueranfly.top/gtnxdnriiw.html

find . -name "*.log" -type f
来源：http://hz.52xcode.cn/gtqbtcmsfc.html

[R44] 按修改时间查找
来源：http://hz.tianlin.xyz/gtzsrvrmst.html

find . -mtime -7 -type f
来源：http://hz.aibaodan.cn/gtwlczjdkz.html

[R45] 批量删除
来源：http://hz.daxiang520.top/gthfadjmgs.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtptfaursm.html

[R46] 递归替换文件内容
来源：http://hz.gotoacloud.top/gtcmqwzcwv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtjdgzhemh.html

[R47] sed 单行替换
来源：http://hz.fzhhl.top/gtiecrjqjb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jqgfzy.top/gtxpurfaep.html

[R48] awk 取指定列
来源：http://hz.316326.xyz/gtrgjfhjia.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenjidiqi.icu/gtsjtqaonc.html

[R49] awk 带条件
来源：http://hz.zhengqikj.top/gthxuekjgp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gteftzgdfk.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gtofzkdtoq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.birdmap.top/gtpqqljtzm.html

[R51] 排序去重取前几
来源：http://hz.guannengcc.top/gtdtlybzau.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxuanxn.top/gtqcldwtxc.html

[R52] 统计行数
来源：http://hz.hysaishi.cn/gtigeexerq.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtsknxtpmz.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtklqhllfy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ehwqpu.com/gtkuwtsvdt.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtsezaevrp.html

diff a.txt b.txt
来源：http://hz.zhaomingkeji.xyz/gtrgumtpbp.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtzqyhtogh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinghuilouyu.cn/gtpwjsxsci.html

[R56] 远程拷贝
来源：http://hz.jinqigfzy.top/gtjphqgvss.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gttfobltml.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gtcpwtbpto.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtvleqomcg.html

[R58] 下载文件
来源：http://hz.tianlin.xyz/gthblpsuuv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtjkhfwirl.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtlasucjmq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yvedp.cn/gtyvzvvgfi.html

[R60] 只看 HTTP 状态码
来源：http://hz.cqqwz.cn/gtwjgjncrg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxinkj.top/gtwjikador.html

[R61] 磁盘占用
来源：http://hz.xinyue.icu/gtmqojzqwj.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtsozfykro.html

[R62] 找最占空间的文件
来源：http://hz.birdmap.top/gtdeqcvddo.html

du -ah . | sort -rh | head -10
来源：http://hz.chenjidiqi.icu/gtwxpaqftc.html

[R63] 内存与进程
来源：http://hz.zhongyouzk.top/gtcbbbrije.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gtwkmeolse.html

[R64] 结束进程
来源：http://hz.hnqzz.top/gtcgmvblty.html

kill -9 $(pgrep -f app.py)
来源：http://hz.0kj1m.cn/gtbmqriskx.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtvpjdqrwn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtlfrgfzpk.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtqiualkmr.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gtidxihdzp.html

[R67] 生成随机十六进制串
来源：http://hz.nanxuanxn.top/gtjhomxhxg.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtzaihcagv.html

[R68] 计算文件校验值
来源：http://hz.hywenlv.cn/gtadgxwqli.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.meibo888.top/gtmtmbsjoj.html

[R69] 生成随机密码
来源：http://hz.gotoacloud.top/gtdmshtkab.html

head -c 16 /dev/urandom | base64
来源：http://hz.aibaodan.cn/gtohzzslgq.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtvhjmmszi.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigufen.top/gthizjtuai.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtletyumoe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zycfv.cn/gtfxqscjnf.html

[R72] 等待端口就绪
来源：http://hz.jqgufenzy.top/gtnhalyliy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhengqikj.top/gtwmxrfqpm.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtbykzokhc.html

split -l 1000 big.log part_
来源：http://hz.sufxvd.cn/gtszfhzeiv.html

[R74] 批量重命名
来源：http://hz.shanyushiyangkeji.top/gtowxlaxwv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yongpay.top/gtffanlrgg.html

[R75] 导出环境变量
来源：http://hz.aizwys.cn/gteaxjhnmc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dianchejie.cn/gtqkixqxef.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtpwsrhfqn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtagljafbd.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtrpmpwgbo.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gttbryaofh.html

[R78] 交互式菜单
来源：http://hz.haohaochexian.top/gtffigldtl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gtourqmdgs.html

[R79] 解析命令行选项
来源：http://hz.yanxiufei.cn/gtkjrktcjo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtvjmuyzxd.html

[R80] 查看脚本执行耗时
来源：http://hz.hnxiangtu.top/gtrwtudrwd.html

time ./run.sh
来源：http://hz.zycfv.cn/gtsovsrmmd.html

================================================================================
来源：http://hz.sxryk.cn/gtoytonokx.html

S. C / C++ 专题
来源：http://hz.jqgfzy.top/gtcrnohzqf.html

================================================================================
来源：http://hz.guowangkeji.top/gttrgcndwe.html

[S01] C：Hello World
来源：http://hz.zhixingplan.top/gttkcweelc.html

#include <stdio.h>
来源：http://hz.jlsjyb.cn/gtqdfujezk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.haohaochexian.top/gtiuzefhby.html

[S02] C：变量与格式化输出
来源：http://hz.ydjk.org.cn/gtwkyivlei.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtrppcnjrm.html

[S03] C：读入整数
来源：http://hz.jinqigufen.top/gtlryijdts.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gtbkdifbje.html

[S04] C：字符串复制
来源：http://hz.zhiwuduotai.top/gtcavbribo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuetiantiany.cn/gtbducdndf.html

[S05] C：字符串长度
来源：http://hz.daxiang520.top/gttefbqqds.html

strlen(s)
来源：http://hz.zhengqikj.top/gtbodxvwrn.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtvrayimbn.html

strcmp(a, b) == 0
来源：http://hz.jqgfzy.top/gtujwyrezv.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gtuiihlnfm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtyvqpghza.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtzrppjmsu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gtwravnebd.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gttwxuszdg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.9152youxi.cn/gttabtbbjd.html

[S10] C：指针与解引用
来源：http://hz.sweek.top/gtqpfghglo.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gteptflequ.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtigqflswh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aibaodan.cn/gtrusdtfub.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jianghu66.top/gtlweshnax.html

fclose(f);
来源：http://hz.bjfxy.top/gtstjyaibn.html

[S12] C：写文件
来源：http://hz.hywenlv.cn/gthafgylcs.html


<!-- 参考信息 -->