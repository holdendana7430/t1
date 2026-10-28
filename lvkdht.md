代发 wailian999

[Q33] 多列分组
来源：http://hz.jinyuanbaomall.cn/gtpjlkczqg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.quarkkingdee.top/gtughejvks.html

[Q34] 每组取第一条
来源：http://hz.ppjwa.cn/gtszqguehu.html

SELECT * FROM (
来源：http://hz.hnqzz.top/gtyrybqlmt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yangfankeji.com/gtqvlrjwix.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtwkvbkvka.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gtcgcnazgl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtpbaumuyr.html

[Q36] 左连接
来源：http://hz.hfpthk.cn/gtbiwiltee.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.haohaochexian.top/gtyoemcrdz.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtlmicsxft.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xingfuxueyuan.xyz/gtmwteqdtk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tianlin.xyz/gtopicshxs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.birdmap.top/gthxstxfpa.html

[Q39] 自连接（查上下级）
来源：http://hz.shzxlz.cn/gtkeedyvjg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigufen.top/gtqljljlji.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hongshengwenyu.top/gtaqanfoxs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xylfe.cn/gtwmiwnofr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fzhhl.top/gtluwbfysu.html

[Q41] 多表连接
来源：http://hz.tanke756.top/gtxkectktm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pengpengdd.cyou/gtsuwuqxni.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dianchejie.cn/gtuwuyhsrq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sweek.top/gtfmkpqfvs.html

[Q42] 连接条件附加过滤
来源：http://hz.zhixingplan.top/gtxxnfagqw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtdmklohou.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.haohaochexian.top/gtrefzsavq.html

[Q43] 标量子查询
来源：http://hz.zdqjudy.top/gtdnpcjqza.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sysykeji.top/gtzcqibizl.html

[Q44] IN 子查询
来源：http://hz.fzhhl.top/gtibsohgmh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhiwuduotai.top/gtngtqvwsr.html

[Q45] EXISTS 判断存在
来源：http://hz.ehwqpu.com/gtxyvygdhe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtpgradokk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.smart0.xyz/gtigsxxend.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtjyeucxyr.html

[Q47] 与平均值比较
来源：http://hz.gogol.net.cn/gtqbvxwbwe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtyovxrvih.html

[Q48] CTE 公用表表达式
来源：http://hz.jyoumei.cn/gtxkyzgghw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.0kj1m.cn/gtznhfuhih.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtsuoavnko.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gtgkjyzvxq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gtrnmhlqzr.html

[Q50] 批量更新
来源：http://hz.tianlin.xyz/gtcaadumpb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtgvqycczt.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtnkhnucju.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shzxlz.cn/gtvrzjaiep.html

[Q52] 删除指定行
来源：http://hz.jiagoushi.top/gtmihklohr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtdymjcgzq.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtpvznhand.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pengpengdd.cyou/gtoodxujep.html

[Q54] 清空表
来源：http://hz.nanxinkj.top/gtkfeehnmq.html

TRUNCATE TABLE logs;
来源：http://hz.ybcxt.top/gtvxfvjklu.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtigdmyuqj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangtech.top/gtwxkbzhrv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gtkzxxvrbi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtuzxdvtel.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtnunnuqxt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.52xcode.cn/gtckpddtkg.html

[Q58] 累计求和
来源：http://hz.zhoulong.xyz/gtvnwsxwrr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtmshwnhlq.html

[Q59] 分组内累计
来源：http://hz.wangshuangyany.cn/gtidjywmjy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.c1oappe.top/gtwcmtiouj.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtlotnrbrf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtviqxpmfw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sysykeji.top/gtcvvhxuox.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gthmptfbau.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jyoumei.cn/gteqnqswsw.html

[Q62] 分组占比
来源：http://hz.cucudq.cn/gtzwxdzcfl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtztrobdyx.html

[Q63] 开启事务
来源：http://hz.52xcode.cn/gtgtvtcpxd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gtxuihlkte.html

[Q64] 提交事务
来源：http://hz.hnqzz.top/gtszgjpgwv.html

COMMIT;
来源：http://hz.hongshengwenyu.top/gtaolkwnvn.html

[Q65] 回滚事务
来源：http://hz.jinqigfzy.top/gtnhydolxr.html

ROLLBACK;
来源：http://hz.jyoumei.cn/gtoayahrlt.html

[Q66] 行锁查询
来源：http://hz.jiagoushi.top/gtyhzmdnow.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtniuuhiat.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtnqirrfef.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gtvsabebun.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gtrgkviokr.html

SAVEPOINT sp1;
来源：http://hz.dashuyun.cn/gtbftiigrm.html

ROLLBACK TO sp1;
来源：http://hz.sufxvd.cn/gtenqkyjpn.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtdtuhobrf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jyoumei.cn/gtofllbcew.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtxnfllrcp.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtmbubkhto.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtahowvotg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gttcvmmwfn.html

[Q72] 查看索引
来源：http://hz.guowangkeji.top/gtvnnpyzjg.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtwymontdg.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtzsnksqab.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnxiangtu.top/gtqzahwhwb.html

[Q74] 强制使用索引
来源：http://hz.chenjidiqi.icu/gtiglxajzw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtdeosguno.html

[Q75] 日期格式化
来源：http://hz.iojbl.cn/gtfgpalqkf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtnwoycfjo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtemtnyuze.html

[Q76] 按天统计
来源：http://hz.haohaochexian.top/gtmxscmaxt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangshuangyany.cn/gtuxlosbxn.html

[Q77] 时间加减
来源：http://hz.sweek.top/gtijnjbxhb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tanke756.top/gtgncvaioh.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtpencjckz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.andypj.xyz/gtmsuxunvy.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtxmlpxkij.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhengqikj.top/gtnfhhgfry.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtshgbscbt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigfzy.top/gtzjdkhtlc.html

[Q81] 字符串替换
来源：http://hz.chenjidiqi.icu/gtxdwqhdex.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtalgkjtvr.html

[Q82] 字符长度与字节长度
来源：http://hz.0kj1m.cn/gtqptilzkb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gotoacloud.top/gtzakpamof.html

[Q83] 大小写转换
来源：http://hz.smart0.xyz/gtghhamipq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ppjwa.cn/gtlsblyjrt.html

[Q84] 去除首尾空格
来源：http://hz.cheryme.top/gtmuxeokcn.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtdpvwgmgn.html

[Q85] 数值取整
来源：http://hz.chenlongwang.top/gtgeeliagv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.feifeiyinyue.top/gtuxbcxzua.html

[Q86] 读取 JSON 字段
来源：http://hz.tian-w.cn/gtbsweioto.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sxryk.cn/gthoudrebi.html

[Q87] JSON 字段做条件
来源：http://hz.gzhubu.top/gtgdppyvna.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gtspsvqqam.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhengqikj.top/gtkkzbwzjn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.mhx1999.top/gtxemtbfax.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinghuilouyu.cn/gtofkgikny.html

[Q89] 判断表是否存在
来源：http://hz.jianghu66.top/gttdtkxkko.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zdqjudy.top/gtvlxojxpm.html

[Q90] 生成序号列
来源：http://hz.sweek.top/gtgesxdnqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yvedp.cn/gtjymjbdca.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoblvedxk.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtmvoggufq.html

================================================================================
来源：http://hz.yueranfly.top/gtqdnwtoai.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gtrsnsekuw.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtldqnyqje.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtrbamuoom.html

[R02] 变量赋值与使用
来源：http://hz.zhixingplan.top/gtbicrsolw.html

name="Tom"; echo "$name"
来源：http://hz.ehwqpu.com/gtfhxulggf.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtgsnnjvvn.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtekbnrdxd.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtrjyjlqid.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.redwolf501.top/gtfxmvdntu.html

[R05] 参数默认值
来源：http://hz.hysaishi.cn/gtoyobeoft.html

name="${1:-default}"
来源：http://hz.zhoulong.xyz/gtegrdbclm.html

[R06] 判断命令是否存在
来源：http://hz.birdmap.top/gtlhhtuvgi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtawgllhvy.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gtdruwdxav.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cucudq.cn/gtuigttqhi.html

[R08] 数值比较
来源：http://hz.zhaomingkeji.xyz/gtpndximdo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dianchejie.cn/gticouqwgb.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtinqtrtms.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenzaomai.com/gtsjpcvtfj.html

[R10] 正则匹配
来源：http://hz.316326.xyz/gtduethbre.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xinyue.icu/gtecyxjpst.html

[R11] case 多分支
来源：http://hz.xziqi.cn/gtzfwcjvya.html

case "$1" in
来源：http://hz.zhengqikj.top/gtfkspzzuc.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtscotlrnx.html

stop)  echo "停止" ;;
来源：http://hz.zhijiandao.cn/gtweokfwvd.html

*)     echo "未知命令" ;;
来源：http://hz.chenjidiqi.icu/gtvrbfuefb.html

esac
来源：http://hz.zhoulong.xyz/gtdblxzjqt.html

[R12] for 遍历文件
来源：http://hz.hnqzz.top/gttjkkjkhu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtbcjseiuk.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtwzgirihi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtpygaifdk.html

[R14] C 风格 for
来源：http://hz.ydzc1.top/gtcvpbdhln.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xziqi.cn/gtizjssspk.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gtgobmhjtu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtwgkidlhf.html

[R16] until 等待条件
来源：http://hz.zycfv.cn/gtzuqjsoye.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ybcxt.top/gtydwosdms.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtfkzokbgm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtrblkuicq.html

[R18] 遍历数组
来源：http://hz.shanyushiyangkeji.top/gtmkftcykr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yvedp.cn/gteidhjoqw.html

[R19] 数组长度
来源：http://hz.daria6918.cn/gtsnizkutv.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtfbxcyhba.html

[R20] 关联数组（字典）
来源：http://hz.jiagoushi.top/gtohgszbqf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj202588.top/gtkqvurahd.html

[R21] 字符串长度
来源：http://hz.c1oappe.top/gtqvdqtlrh.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtfypbjpsg.html

[R22] 截取子串
来源：http://hz.dianchejie.cn/gtfywjjbfy.html

echo "${s:0:5}"
来源：http://hz.sweek.top/gtxnlvfwnd.html

[R23] 字符串替换
来源：http://hz.jlsjyb.cn/gthotfaifg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gteohcyrrh.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gttxtesdmo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gtikxxnuhp.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtbycwyaua.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gtjmogqsbm.html

[R26] 命令替换
来源：http://hz.hywenlv.cn/gtcnleesks.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtzsquhbkn.html

[R27] 算术展开
来源：http://hz.redwolf501.top/gturkrzcuf.html

echo $((1 + 2 * 3))
来源：http://hz.xziqi.cn/gtseuwkfny.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtucywsjjv.html

echo "scale=2; 10/3" | bc
来源：http://hz.xziqi.cn/gtnnflpkxh.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtqhhfrpdw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fzhhl.top/gterjukptw.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtxpydkevg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.kuanghao11.cn/gtvtafnxdf.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtwmzwmyja.html

f() { local x=1; echo "$x"; }
来源：http://hz.ppjwa.cn/gtwatdscxk.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtaftlavbp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.c1oappe.top/gtpuoydiij.html

[R33] 捕获错误并提示行号
来源：http://hz.sysykeji.top/gtcloebfda.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hnqzz.top/gttzjsaicy.html

[R34] 退出时清理
来源：http://hz.sysykeji.top/gtnzublwlh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtuhvxfbgn.html

[R35] 后台执行并等待
来源：http://hz.haohaochexian.top/gttaubvwxz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgfzy.top/gtrtwqfcxa.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtwsdltaut.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtdzzbugiy.html

[R37] 把输出赋给变量
来源：http://hz.zhaomingkeji.xyz/gtqecoeopl.html

files=$(ls -1)
来源：http://hz.sufxvd.cn/gtgetxxwcs.html

[R38] 管道串联
来源：http://hz.vqdsnc.cn/gtxfqqxkyh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtzhjdgzll.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtqzqzbccc.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtcwdfkrdt.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtvyvbfecc.html

echo "log" >> out.log
来源：http://hz.nwbrower.top/gtfsllpgsl.html

[R41] 丢弃输出
来源：http://hz.sweek.top/gtfgogjfxn.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtdwrjfvjj.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gtbtdkssrp.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gteokfilkv.html

[R43] 按名字查找文件
来源：http://hz.xuetiantiany.cn/gtyrgynvje.html

find . -name "*.log" -type f
来源：http://hz.pengpengdd.cyou/gthmqhsjjx.html

[R44] 按修改时间查找
来源：http://hz.gogol.net.cn/gtgcqvxjdz.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gthqtlbwze.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gttqwemhmr.html

find . -name "*.tmp" -delete
来源：http://hz.yueranfly.top/gtafhdppoq.html

[R46] 递归替换文件内容
来源：http://hz.hnqzz.top/gtxfipnqmp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenlongwang.top/gtcviycwge.html

[R47] sed 单行替换
来源：http://hz.ybcxt.top/gtazoppnep.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gttngwpgiq.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtzheexeol.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gtisrsrqla.html

[R49] awk 带条件
来源：http://hz.ppjwa.cn/gtmatgqdgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtzwftkyxw.html

[R50] awk 求和
来源：http://hz.jyoumei.cn/gtiohjjgnx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtudffhwhx.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtxfgotmci.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.bjfxy.top/gtzhpoazrg.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gtrcdzggmt.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gtqxctpgbw.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtqzdruyed.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinghuilouyu.cn/gtrasgaxbr.html

[R54] 比较两个文件
来源：http://hz.jinqigufen.top/gtlidjtcag.html

diff a.txt b.txt
来源：http://hz.xylfe.cn/gtlynddzrd.html

[R55] 压缩与解压
来源：http://hz.yuanzhike.top/gtbmgtqqau.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhijiandao.cn/gtopoysieg.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtwlzdbmwc.html

scp file user@host:/path/
来源：http://hz.tianlin.xyz/gtnkfcdvjn.html

[R57] 远程执行命令
来源：http://hz.xingfuxueyuan.xyz/gtfykbvwio.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gtfdpwvyvh.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtdgysgqcn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtaxciduoj.html

[R59] 发 POST JSON
来源：http://hz.xuanzx.com/gtrgbdlkbc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtpocwjcnd.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtnjlsdlqm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnqzz.top/gtwnfihega.html

[R61] 磁盘占用
来源：http://hz.pycfn.com/gtgupdunfg.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gtrowtytoz.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtksymkwra.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtsaotohja.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtcihrearo.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtsrfgdckh.html

[R64] 结束进程
来源：http://hz.redwolf501.top/gtiwokcngu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtmufwgetu.html

[R65] 查看端口占用
来源：http://hz.ehwqpu.com/gtxgiewhyq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtullbrjck.html

[R66] 定时任务
来源：http://hz.chenjidiqi.icu/gtnihnrjvv.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gtnhfgwuew.html

[R67] 生成随机十六进制串
来源：http://hz.kuanghao11.cn/gtxzfdogji.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtkyktddkt.html

[R68] 计算文件校验值
来源：http://hz.xuanzx.com/gtjwvumnws.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.kuanghao11.cn/gtobicoppw.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtwazymgfz.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenzaomai.com/gtuhdvefri.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtlzmacwzu.html

date +%s;  date -d @1700000000
来源：http://hz.cheryme.top/gtoxlvgoll.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtpubocwyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtwdykglis.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtjbvzxcfr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtwroimvwz.html

[R73] 分割大日志
来源：http://hz.sxryk.cn/gtxhszhonu.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtpugoiuql.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtvaisrzjm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gthxrfnpnf.html

[R75] 导出环境变量
来源：http://hz.shuidangran.top/gtzgbxzjuz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zdqjudy.top/gtscgewwir.html

[R76] 使用临时文件
来源：http://hz.zhiwuduotai.top/gtxgbvcwbm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtdkpogibw.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gtrxdwrles.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtnwmyqbxk.html

[R78] 交互式菜单
来源：http://hz.yanxiufei.cn/gtiuvzoawm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuetiantiany.cn/gtfxamlmzc.html

[R79] 解析命令行选项
来源：http://hz.jianghu66.top/gtkovjdwrl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtivjnmksp.html

[R80] 查看脚本执行耗时
来源：http://hz.jiagoushi.top/gtdjhpgwzz.html

time ./run.sh
来源：http://hz.havefunace.top/gtrtohkous.html

================================================================================
来源：http://hz.hfpthk.cn/gtdzouwxxh.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gtqejmxdcj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtzoxguqyb.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtddcpdstt.html

#include <stdio.h>
来源：http://hz.zhongyouzk.top/gtyabnrrzl.html


<!-- 参考信息 -->