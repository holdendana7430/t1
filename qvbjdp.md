代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gtxpyncpof.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.andypj.xyz/gtxxrhbmdw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gthpcwvjdr.html

[Q41] 多表连接
来源：http://hz.hammf.cn/gtcnfldzql.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtljmcdnoc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgfzy.top/gtbxkvwxdm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dashuyun.cn/gtkcflqdze.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtspdumlba.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gthumelggv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ivvv.top/gtzqkushzj.html

[Q43] 标量子查询
来源：http://hz.kuanghao11.cn/gtukufswwh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtimqkxdee.html

[Q44] IN 子查询
来源：http://hz.ppjwa.cn/gtffafcujq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sxryk.cn/gtevhgifrv.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gttyystilf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtxscfxtfz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.mhx1999.top/gtoadfbpbc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtzvcbnxcu.html

[Q47] 与平均值比较
来源：http://hz.nwbrower.top/gtpppwhbmj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtmxwjhfwa.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtayyxvlsx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xingfuxueyuan.xyz/gtjdbtoepx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shangyingyoupin.top/gtrauxohpn.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtehnlndyz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtilrettuy.html

[Q50] 批量更新
来源：http://hz.jqgfzy.top/gtrqavcjjj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cdnleiting.top/gtavogxkzw.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtlmfdkaqh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zycfv.cn/gtmlvjyxzf.html

[Q52] 删除指定行
来源：http://hz.hnqzz.top/gtfreeyjbo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtmfnkkwzm.html

[Q53] 按条件删除
来源：http://hz.ydzc1.top/gtflqhzxii.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yueranfly.top/gtebixohvs.html

[Q54] 清空表
来源：http://hz.yj20258888.top/gtoshvvjvj.html

TRUNCATE TABLE logs;
来源：http://hz.birdmap.top/gtduvqjaeb.html

[Q55] 排名（并列占位）
来源：http://hz.nanxuanxn.top/gtkhpmkwfr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtocufmtct.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigfzy.top/gttqymxxum.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shangyingyoupin.top/gtwyruxwqg.html

[Q57] 行号
来源：http://hz.nanxinkj.top/gteiraqbwl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtoodmgewx.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtikkxwnca.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtqeqrcywq.html

[Q59] 分组内累计
来源：http://hz.c1oappe.top/gtnckfpinp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gtlahpaeop.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gtdrspfuwc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cashguo.top/gtomxfmhcx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtksfodsnv.html

[Q61] 移动平均
来源：http://hz.havefunace.top/gtiixbbusu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258.top/gtxkxhynqf.html

[Q62] 分组占比
来源：http://hz.daria6918.cn/gtctjptsbt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtxxwfervf.html

[Q63] 开启事务
来源：http://hz.chenlongwang.top/gtdexhuqhr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gzhubu.top/gtvdozkike.html

[Q64] 提交事务
来源：http://hz.havefunace.top/gtuquewcqf.html

COMMIT;
来源：http://hz.gotoacloud.top/gtejbbwxlt.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtrdvmsjvx.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtzbsptzfg.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtvgnkdvtf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gtffdgbsor.html

[Q67] 设置隔离级别
来源：http://hz.pengpengdd.cyou/gtvxdfapgl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydjk.org.cn/gtaixqfjjn.html

[Q68] 保存点
来源：http://hz.shanyushiyangkeji.top/gtnmjdxyen.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtgbubixwg.html

ROLLBACK TO sp1;
来源：http://hz.ehwqpu.com/gtpaeopfjv.html

[Q69] 查看执行计划
来源：http://hz.zhaomingkeji.xyz/gtmvosrxqx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xylfe.cn/gthqccowha.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gtizhusjto.html

ANALYZE TABLE users;
来源：http://hz.jinqigfzy.top/gtluvvxbzc.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gtgxjsydls.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtrifwltjc.html

[Q72] 查看索引
来源：http://hz.svipenyu.cn/gtkenykxku.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtoxqucqcy.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtajhigemr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangshuangyany.cn/gttbzbxbck.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtzlxgggbv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtsqhyfwbd.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtzwtakune.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtkbqkmdlo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guowangkeji.top/gtslfxemrh.html

[Q76] 按天统计
来源：http://hz.fzhhl.top/gttadiraso.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yonumen.top/gtnfhcjvab.html

[Q77] 时间加减
来源：http://hz.shzxlz.cn/gtieivchcc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtpywnpega.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtylrnzlwz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gtyztwvnzy.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtzroiarcq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangshuangyany.cn/gtktnlwkoa.html

[Q80] 字符串截取
来源：http://hz.nwbrower.top/gtsnbqxlfq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xziqi.cn/gtwgykolbz.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtlhwmpqqe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtshwhxooi.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtjmqejllw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtdzkuvgap.html

[Q83] 大小写转换
来源：http://hz.haohaochexian.top/gtmuqeouzf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.meibo888.top/gtebdnsobo.html

[Q84] 去除首尾空格
来源：http://hz.mhx1999.top/gtjnlktgbu.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxinkj.top/gtdxegzspt.html

[Q85] 数值取整
来源：http://hz.jqgfzy.top/gtksmcsliy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xinyue.icu/gtrxjjdzwe.html

[Q86] 读取 JSON 字段
来源：http://hz.hnqzz.top/gtqpbjiqte.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtnaokojgv.html

[Q87] JSON 字段做条件
来源：http://hz.jlsjyb.cn/gtnczsdkvo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cashguo.top/gtjggrdqqp.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj202588.top/gtdlhynrqz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sxryk.cn/gtzgdnwdrg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.feifeiyinyue.top/gtllnutjus.html

[Q89] 判断表是否存在
来源：http://hz.sysykeji.top/gtgvednpgo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnxiangtu.top/gtdrxxoobj.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtjunzrias.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xziqi.cn/gtjllgvitp.html

================================================================================
来源：http://hz.zhixingplan.top/gtvzixkzoo.html

R. Bash 专题
来源：http://hz.cqqwz.cn/gtbkomghub.html

================================================================================
来源：http://hz.ppjwa.cn/gtgqwfqbok.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtbbrykzei.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtmgnattdr.html

set -euo pipefail
来源：http://hz.tianlin.xyz/gtnfuxdkal.html

[R02] 变量赋值与使用
来源：http://hz.ehwqpu.com/gtsjexkuka.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtfryizwna.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gtkefhnxyv.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gtpifrrpky.html

[R04] 位置参数
来源：http://hz.sxryk.cn/gtqrsjfpom.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtrywxzpta.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gttfeyzrld.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gtxmhqxbnl.html

[R06] 判断命令是否存在
来源：http://hz.hammf.cn/gtxeblbnrm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenlongwang.top/gtmyginofm.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gtxsbagxmo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jianghu66.top/gtpjpxjwfl.html

[R08] 数值比较
来源：http://hz.sxryk.cn/gtdxglvhwy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ppjwa.cn/gtpzclzwcs.html

[R09] 字符串比较
来源：http://hz.tian-w.cn/gtqtqxdftl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fzhhl.top/gtsozjviqd.html

[R10] 正则匹配
来源：http://hz.0kj1m.cn/gtybayfftz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gtesvkqicr.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtopjbjbeq.html

case "$1" in
来源：http://hz.316326.xyz/gtaszwzfpf.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtbtfwhjpp.html

stop)  echo "停止" ;;
来源：http://hz.sufxvd.cn/gtpzfsgvky.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtmryaxblc.html

esac
来源：http://hz.gogol.net.cn/gtxuzoggel.html

[R12] for 遍历文件
来源：http://hz.hywenlv.cn/gtsjxvblcu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.smart0.xyz/gtmriqsmfb.html

[R13] for 计数循环
来源：http://hz.gogol.net.cn/gtydqkdhuo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuanzx.com/gtrxqpgglr.html

[R14] C 风格 for
来源：http://hz.andypj.xyz/gtwxjljxao.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtcniklglu.html

[R15] while 逐行读文件
来源：http://hz.xuanzx.com/gthsuxpalp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yangfankeji.com/gtkimiximb.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtmvwbpfta.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtpvmzswrt.html

[R17] 数组定义与取值
来源：http://hz.xylfe.cn/gtgmngbaji.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258888.top/gtalanrnui.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtjsfhcvwe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aibaodan.cn/gtoolkjihk.html

[R19] 数组长度
来源：http://hz.hongshengwenyu.top/gtluyamczw.html

echo "${#arr[@]}"
来源：http://hz.xuetiantiany.cn/gtppmywkfa.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtviyodqzp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtsuwxqwcb.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtyaqeqecf.html

echo "${#s}"
来源：http://hz.hongshengwenyu.top/gtfauxprbn.html

[R22] 截取子串
来源：http://hz.yangfankeji.com/gtxcmnaizp.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtxnidkhoe.html

[R23] 字符串替换
来源：http://hz.daxiang520.top/gtgwmrvnzs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tian-w.cn/gtpriqptsm.html

[R24] 大小写转换
来源：http://hz.yuanzhike.top/gtedrhvcun.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtytmcwzbs.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigufen.top/gtapqmfwdm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenjidiqi.icu/gtaqnmcbep.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtschodcdw.html

now=$(date +%F); echo "$now"
来源：http://hz.yangfankeji.com/gtbwlwfipw.html

[R27] 算术展开
来源：http://hz.hysaishi.cn/gtpsswmlmb.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtckzznprn.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gtptehjadr.html

echo "scale=2; 10/3" | bc
来源：http://hz.0kj1m.cn/gteeypbcrq.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gtmflatpmc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtucgeuzwv.html

[R30] 函数返回状态码
来源：http://hz.tianlin.xyz/gtbujfrxdd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guannengcc.top/gtqnpsosje.html

[R31] 局部变量
来源：http://hz.cheryme.top/gtlnqjkkvz.html

f() { local x=1; echo "$x"; }
来源：http://hz.daria6918.cn/gtyyznoscz.html

[R32] 参数个数校验
来源：http://hz.haohaochexian.top/gtviicifii.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtqrbwgwqg.html

[R33] 捕获错误并提示行号
来源：http://hz.dashuyun.cn/gttrcrixmh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtvodesolg.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtdixvontx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gttfknlmpr.html

[R35] 后台执行并等待
来源：http://hz.quarkkingdee.top/gteesdhwps.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gaohongyu789.top/gtykpdhiil.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtorpastss.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.iojbl.cn/gtwwoohtgb.html

[R37] 把输出赋给变量
来源：http://hz.chenlongwang.top/gtyvtsydkx.html

files=$(ls -1)
来源：http://hz.ivvv.top/gtttqkckgx.html

[R38] 管道串联
来源：http://hz.sufxvd.cn/gtyejevgjg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtpkseulzc.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gtanhzccln.html

cmd > out.log 2>&1
来源：http://hz.dashuyun.cn/gtwivlqjtz.html

[R40] 追加写日志
来源：http://hz.yj202588.top/gtbxltphra.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtqzcwmqkx.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtbzhxaimz.html

cmd >/dev/null 2>&1
来源：http://hz.zhixingplan.top/gthsvryrvy.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtkzddsqmp.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtkwhyslvw.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtxmhazzwa.html

find . -name "*.log" -type f
来源：http://hz.sysykeji.top/gttfyswvef.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtwpiydcyy.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtpifwfxph.html

[R45] 批量删除
来源：http://hz.gaohongyu789.top/gtovtfmyhm.html

find . -name "*.tmp" -delete
来源：http://hz.sxryk.cn/gtcvbhmxli.html

[R46] 递归替换文件内容
来源：http://hz.iojbl.cn/gtngnwsmxt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gogol.net.cn/gthergqven.html

[R47] sed 单行替换
来源：http://hz.jinqigfzy.top/gtizitbcav.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.0kj1m.cn/gticaaqaqj.html

[R48] awk 取指定列
来源：http://hz.9152youxi.cn/gttwtqblio.html

awk '{print $1, $3}' a.txt
来源：http://hz.cucudq.cn/gtjdyaapjj.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtsakwmvam.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtryofhtbd.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtwlvcvmfh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtfisbrbxx.html

[R51] 排序去重取前几
来源：http://hz.cucudq.cn/gtekhnplit.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sufxvd.cn/gtfajqumpr.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gtafwjkrbr.html

wc -l a.txt
来源：http://hz.xziqi.cn/gtbmboyurb.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gtfyoppeuq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.316326.xyz/gtixabprfb.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtdydviwnc.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtnuhkgmtx.html

[R55] 压缩与解压
来源：http://hz.hywenlv.cn/gtmasqrwwy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtoatenxjj.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtmfqoupic.html

scp file user@host:/path/
来源：http://hz.yuanzhike.top/gtdvigdcdv.html

[R57] 远程执行命令
来源：http://hz.aizwys.cn/gtjdeshbmm.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtemngkqkj.html

[R58] 下载文件
来源：http://hz.jiagoushi.top/gtsglhvwch.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtvvcktybm.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtdimsxzbc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tanke756.top/gtkwtyknqg.html

[R60] 只看 HTTP 状态码
来源：http://hz.pycfn.com/gtbhttnazb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtiifrebvi.html

[R61] 磁盘占用
来源：http://hz.sxryk.cn/gtdstttqma.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtrlxmaxbk.html

[R62] 找最占空间的文件
来源：http://hz.andypj.xyz/gtgvetlwws.html

du -ah . | sort -rh | head -10
来源：http://hz.xuanzx.com/gtaqjvrgac.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtmtqpypjd.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gtxirnwmtl.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtyjtiusgn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gtepmsvxve.html

[R65] 查看端口占用
来源：http://hz.cashguo.top/gttnkibynp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.vqdsnc.cn/gtgqtlsbli.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtvjkbqllj.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gtqjurldbx.html

[R67] 生成随机十六进制串
来源：http://hz.shangyingyoupin.top/gtselefnap.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gtnkevxfvm.html

[R68] 计算文件校验值
来源：http://hz.guowangkeji.top/gtlupbwcsy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sweek.top/gtarslxwzg.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtumoklfnk.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgufenzy.top/gtixxhiydb.html

[R70] 时间戳与互转
来源：http://hz.sxryk.cn/gtqgylsdyj.html

date +%s;  date -d @1700000000
来源：http://hz.jlsjyb.cn/gtagddhuhf.html

[R71] 日期格式化
来源：http://hz.guannengcc.top/gtazqftpzi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cucudq.cn/gtfjgszuce.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtlztmwdbr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.316326.xyz/gtlahcnyor.html

[R73] 分割大日志
来源：http://hz.kuanghao11.cn/gtkuxmeorr.html

split -l 1000 big.log part_
来源：http://hz.nwbrower.top/gtnnwsghkd.html

[R74] 批量重命名
来源：http://hz.nanxuanxn.top/gtfgdvycns.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daria6918.cn/gtypejnutn.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtpqkapwpq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtbeowrfbj.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gtpbhvjvmx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtmhjmhsuo.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gtqrrpudia.html

read -rp "请输入: " ans
来源：http://hz.jlsjyb.cn/gtazaginsl.html

[R78] 交互式菜单
来源：http://hz.sysykeji.top/gtlmzcjkxf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuxming.cn/gtigcklcfl.html

[R79] 解析命令行选项
来源：http://hz.gzhubu.top/gtnigtiktg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtxobtmdmv.html

[R80] 查看脚本执行耗时
来源：http://hz.xinyue.icu/gtjiupxjcb.html

time ./run.sh
来源：http://hz.gzhubu.top/gtxkyjmwbx.html

================================================================================
来源：http://hz.xziqi.cn/gtmbamvziq.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gtzjakgnqb.html

================================================================================
来源：http://hz.yueranfly.top/gtkdaokcjg.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gthayhjyge.html

#include <stdio.h>
来源：http://hz.tanke756.top/gtctylzsdc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinghuilouyu.cn/gtvjwvkqif.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gthryaqvkb.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydjk.org.cn/gtrieeizbl.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtfxvmyxov.html

int x; scanf("%d", &x);
来源：http://hz.hongshengwenyu.top/gtwlfmilxa.html

[S04] C：字符串复制
来源：http://hz.dianchejie.cn/gtsgtkobcf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hfpthk.cn/gtyhvxxmjf.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtagdhwubc.html

strlen(s)
来源：http://hz.nwbrower.top/gtjfjxeajn.html

[S06] C：字符串比较
来源：http://hz.daxiang520.top/gtgijetlrt.html

strcmp(a, b) == 0
来源：http://hz.mhx1999.top/gtlfelwqsc.html

[S07] C：数组遍历求和
来源：http://hz.guannengcc.top/gtjmhrvcej.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangshuangyany.cn/gtwmotuspx.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtogrvryhk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnqzz.top/gtsifxqfnc.html

[S09] C：结构体定义与初始化
来源：http://hz.dashuyun.cn/gtkilzqgqo.html


<!-- 参考信息 -->