代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ivvv.top/gtfuxqhqfy.html

[Q30] 分组统计
来源：http://hz.jyoumei.cn/gtwyfjaxok.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtfqmgprbm.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gtzpvtyzdb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigfzy.top/gtjjpiaiaw.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtqjpzjuja.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtphhbbnmq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gotoacloud.top/gteseyyuen.html

[Q33] 多列分组
来源：http://hz.ivvv.top/gtxtpvesfm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dashuyun.cn/gtxokiprvz.html

[Q34] 每组取第一条
来源：http://hz.ydjk.org.cn/gtwkszjusl.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtkpzlhwys.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuxming.cn/gtzerdyxkf.html

) t WHERE rn = 1;
来源：http://hz.hammf.cn/gtutymssjf.html

[Q35] 内连接
来源：http://hz.316326.xyz/gtrxozplfp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtwqfwdjkq.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gtcjtjzabt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtikizncza.html

[Q37] 右连接
来源：http://hz.yj202588.top/gteavkavvm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gthdzsymlr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtqozhpnld.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtzpsvsmly.html

[Q39] 自连接（查上下级）
来源：http://hz.hywenlv.cn/gtsshqkkyg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenjidiqi.icu/gtzzgzdfff.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gtswaarhqv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gtfpqukwlv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtaqcgqjmw.html

[Q41] 多表连接
来源：http://hz.sxryk.cn/gtdcakpigo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258.top/gtzteinmzy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sweek.top/gtlgmggwig.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtbaknrwlv.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtbipqhmra.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cheryme.top/gtvizxrofa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fengsongda.top/gtgagtfbzz.html

[Q43] 标量子查询
来源：http://hz.0kj1m.cn/gtyzqhqnba.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtjdykpgbq.html

[Q44] IN 子查询
来源：http://hz.quarkkingdee.top/gtpwuhxytd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgfzy.top/gtmcxsfyeq.html

[Q45] EXISTS 判断存在
来源：http://hz.birdmap.top/gtenymezfv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtgbaypatx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sufxvd.cn/gtpjbradgn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtdwxvoudn.html

[Q47] 与平均值比较
来源：http://hz.shangyingyoupin.top/gtzisokodc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenzaomai.com/gtfpniaquo.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxinkj.top/gtulfkpzwu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.bjfxy.top/gtyzyyghas.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gthbktuhhi.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtcwnwhzqc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtuduwlwnc.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtfobbruvv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hongshengwenyu.top/gtzptsydrj.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtqulfygzh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jianghu66.top/gtnihnrcty.html

[Q52] 删除指定行
来源：http://hz.zhoulong.xyz/gtxquqfeio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtstpjltny.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtmjsqtlyd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtgkuvxvus.html

[Q54] 清空表
来源：http://hz.yj20258888.top/gtbfbnndnj.html

TRUNCATE TABLE logs;
来源：http://hz.dashuyun.cn/gtvxqmlvfw.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtusbffdbm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gtqqhmsspv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jiagoushi.top/gtvvenaxwd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258.top/gtyladfqvw.html

[Q57] 行号
来源：http://hz.316326.xyz/gtsvtwvwpu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenjidiqi.icu/gtahinjbtr.html

[Q58] 累计求和
来源：http://hz.hfpthk.cn/gthrffslrb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtpdqtjhym.html

[Q59] 分组内累计
来源：http://hz.jiagoushi.top/gtknczfrft.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtsnbsgyit.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtrdgipobi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.0kj1m.cn/gtwaxuxbit.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtrqewztrp.html

[Q61] 移动平均
来源：http://hz.ybcxt.top/gtogtfvswm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xziqi.cn/gtgnsmgdug.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtrytixxeq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtugcdotnk.html

[Q63] 开启事务
来源：http://hz.iojbl.cn/gtxeklnxtc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangshuangyany.cn/gtzmijcyyv.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtrkqiycpk.html

COMMIT;
来源：http://hz.yj20258.top/gtxrsjsjjh.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtysnmwlkd.html

ROLLBACK;
来源：http://hz.sysykeji.top/gtqrfvyrzq.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtpjvmmulw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sweek.top/gtaawgwfwm.html

[Q67] 设置隔离级别
来源：http://hz.gogol.net.cn/gtuawaehdh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtjsgxrdav.html

[Q68] 保存点
来源：http://hz.tian-w.cn/gtwfbnbgps.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtughjyzrv.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtpafxxsyn.html

[Q69] 查看执行计划
来源：http://hz.gotoacloud.top/gtwurumayt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtydycmwqj.html

[Q70] 更新统计信息
来源：http://hz.nanxuanxn.top/gtxdtehyvp.html

ANALYZE TABLE users;
来源：http://hz.jqgfzy.top/gtrnnthjch.html

[Q71] 查看建表语句
来源：http://hz.guannengcc.top/gtmsmvvgfd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtzmpupozg.html

[Q72] 查看索引
来源：http://hz.9152youxi.cn/gtwonuzkzw.html

SHOW INDEX FROM users;
来源：http://hz.nanxinkj.top/gtenetnfrf.html

[Q73] 查看表状态
来源：http://hz.gotoacloud.top/gtwvmassud.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.vqdsnc.cn/gtpviyvfgu.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtzdogaydi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtxwalunyt.html

[Q75] 日期格式化
来源：http://hz.tianlin.xyz/gtvvwrudxp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gtyyaergdk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gtfrwcdsmy.html

[Q76] 按天统计
来源：http://hz.xinyue.icu/gthmzhuhhi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxinkj.top/gteydzfowz.html

[Q77] 时间加减
来源：http://hz.jinqigufen.top/gtuymytmih.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtckrxpjcc.html

[Q78] 当前时间
来源：http://hz.ppjwa.cn/gtefeuajli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hfpthk.cn/gterpjxzcs.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtiyqpjzeh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jlsjyb.cn/gtysalljuv.html

[Q80] 字符串截取
来源：http://hz.zdqjudy.top/gtjnyeixlp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yangfankeji.com/gtowvhooje.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gtamiaxcsm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtqlmvedcp.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtusbttsdv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ivvv.top/gtjfjlmkio.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtjzajltki.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shuidangran.top/gtecgukori.html

[Q84] 去除首尾空格
来源：http://hz.zhoulong.xyz/gtaajvquvk.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtjdwjixed.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gthvurqcfb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuanzhike.top/gtdeennnuw.html

[Q86] 读取 JSON 字段
来源：http://hz.shuidangran.top/gtzpyenmpl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtalecrjeg.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtnzdjufat.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtghsidslz.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtrckenxxb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtsdwtgpbr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jyoumei.cn/gtvptxjaap.html

[Q89] 判断表是否存在
来源：http://hz.xuetiantiany.cn/gtglvjllmg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtwltmsqxa.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtznizfuxt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gtsubkpmrn.html

================================================================================
来源：http://hz.aibaodan.cn/gtzwhztphx.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gttvxqqwvj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthtcbnnle.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gttpdulkiu.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtsxxiipvv.html

set -euo pipefail
来源：http://hz.jinqigufen.top/gtcjhpwieu.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtcqobzgmk.html

name="Tom"; echo "$name"
来源：http://hz.xziqi.cn/gtjnpngpcd.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtrrnagcyo.html

readonly PI=3.14
来源：http://hz.c1oappe.top/gtaujtsxcu.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtlcvkiioo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ppjwa.cn/gtdiddqika.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gttimdfhwv.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtyjwuymkk.html

[R06] 判断命令是否存在
来源：http://hz.jinyuanbaomall.cn/gtntltgdwx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jyoumei.cn/gttetoiaci.html

[R07] if 判断文件
来源：http://hz.c1oappe.top/gtudckwrrv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daxiang520.top/gtmuaoslba.html

[R08] 数值比较
来源：http://hz.hysaishi.cn/gtwlzjldro.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtibebgqzy.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtxguelmwv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtpsqhrucu.html

[R10] 正则匹配
来源：http://hz.iojbl.cn/gtovsxcfto.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtgubahuxw.html

[R11] case 多分支
来源：http://hz.andypj.xyz/gteogmtfpu.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtmcuqrimr.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gtzularkhl.html

stop)  echo "停止" ;;
来源：http://hz.fzhhl.top/gtxtxjbxug.html

*)     echo "未知命令" ;;
来源：http://hz.gzhubu.top/gtrvatcjzn.html

esac
来源：http://hz.yangfankeji.com/gtircechpz.html

[R12] for 遍历文件
来源：http://hz.svipenyu.cn/gtccsiawkq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gttlxauniu.html

[R13] for 计数循环
来源：http://hz.guowangkeji.top/gtykksnhgm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.birdmap.top/gtjiqtmemi.html

[R14] C 风格 for
来源：http://hz.zhongyouzk.top/gtbcgoruaj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yanxiufei.cn/gteyiqwmrc.html

[R15] while 逐行读文件
来源：http://hz.zhixingplan.top/gtycyzjtaj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gtlufscdex.html

[R16] until 等待条件
来源：http://hz.ydjk.org.cn/gtsnjcpamj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cqqwz.cn/gtkdoswoid.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtogdkkpoo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gtmuozwrah.html

[R18] 遍历数组
来源：http://hz.redwolf501.top/gtesivqypr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xziqi.cn/gtnkhtfwnw.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gthjamohqp.html

echo "${#arr[@]}"
来源：http://hz.wangdashe.top/gtjrcszwag.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtnhfffjxv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aizwys.cn/gtgqwqgvad.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtyvfzsnol.html

echo "${#s}"
来源：http://hz.xuanzx.com/gtudxxghkk.html

[R22] 截取子串
来源：http://hz.hfpthk.cn/gtyszbykua.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gthwzhhcdr.html

[R23] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtwobwndxo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtohihvwnx.html

[R24] 大小写转换
来源：http://hz.tanke756.top/gtotdumsxo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtoxqlkejz.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinghuilouyu.cn/gtvmkczwum.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuxming.cn/gtjczyzghk.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtlzavoqyg.html

now=$(date +%F); echo "$now"
来源：http://hz.guannengcc.top/gttqecvhcm.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gtqkjupjfg.html

echo $((1 + 2 * 3))
来源：http://hz.jinqigfzy.top/gtvhnjcxow.html

[R28] 浮点运算
来源：http://hz.zdqjudy.top/gtjnwkvwax.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gtlewwtpln.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtymdaqizi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtupgimwfw.html

[R30] 函数返回状态码
来源：http://hz.zhiwuduotai.top/gteiwicnha.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tianlin.xyz/gtvyvyfahs.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gthngdvmka.html

f() { local x=1; echo "$x"; }
来源：http://hz.shzxlz.cn/gtwsesahco.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtzafnagwk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ehwqpu.com/gtszeifffv.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtjjkfoima.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtsnrtvlzr.html

[R34] 退出时清理
来源：http://hz.hfpthk.cn/gtjllzxzui.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gtwaesdlfj.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gthftkhvao.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pengpengdd.cyou/gtuswvzigl.html

[R36] 并发执行多个任务
来源：http://hz.zhixingplan.top/gtyqfmyqja.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gtcekfgzfs.html

[R37] 把输出赋给变量
来源：http://hz.zhengqikj.top/gtqscyeiho.html

files=$(ls -1)
来源：http://hz.feifeiyinyue.top/gtqqywgadm.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtaajgrmyu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.havefunace.top/gtnktjfepf.html

[R39] 重定向标准输出与错误
来源：http://hz.xuetiantiany.cn/gtoxoxtsvn.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtgewrytgc.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtyxfadvxd.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtrxxihntp.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gthgrzxpfy.html

cmd >/dev/null 2>&1
来源：http://hz.xuanzx.com/gtudqeldle.html

[R42] 输入重定向
来源：http://hz.yangfankeji.com/gtefdelqex.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gttttomgux.html

[R43] 按名字查找文件
来源：http://hz.zhiwuduotai.top/gtkibgbldn.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gthtdouohg.html

[R44] 按修改时间查找
来源：http://hz.bjfxy.top/gtmfnhnghl.html

find . -mtime -7 -type f
来源：http://hz.zycfv.cn/gtajxcbrfx.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gtxcenfmbm.html

find . -name "*.tmp" -delete
来源：http://hz.cdnleiting.top/gtfnzlakvl.html

[R46] 递归替换文件内容
来源：http://hz.jianghu66.top/gtnymhcxbl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtyskbpfye.html

[R47] sed 单行替换
来源：http://hz.cucudq.cn/gtcdrmidvy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gaohongyu789.top/gtvccephsn.html

[R48] awk 取指定列
来源：http://hz.yueranfly.top/gtiboxfafc.html

awk '{print $1, $3}' a.txt
来源：http://hz.yangfankeji.com/gtnuzntwbg.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtblrxjyim.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtgelbmyix.html

[R50] awk 求和
来源：http://hz.fengsongda.top/gthhmsqrpv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtyjmgydzw.html

[R51] 排序去重取前几
来源：http://hz.meibo888.top/gtikpazxoe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtosmnpluw.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtitbtxhrf.html

wc -l a.txt
来源：http://hz.meibo888.top/gtbvxpbdud.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtfdtywcbk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigufen.top/gtqgjskyei.html

[R54] 比较两个文件
来源：http://hz.yuxming.cn/gtingvtwup.html

diff a.txt b.txt
来源：http://hz.daxiang520.top/gtcapvmpnd.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtadvgbryt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yongpay.top/gtdaurvlpc.html

[R56] 远程拷贝
来源：http://hz.jlsjyb.cn/gtscffkjly.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtxxgjzixb.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangtech.top/gtbcukcaiy.html

ssh user@host 'uptime'
来源：http://hz.nanxinkj.top/gtpgxhkyzi.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtftnjdaqd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gtpkcorymb.html

[R59] 发 POST JSON
来源：http://hz.zhijiandao.cn/gtcmusnmhj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtwinboqhm.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuanzx.com/gtklywzant.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.c1oappe.top/gtdgprtcgm.html

[R61] 磁盘占用
来源：http://hz.sxryk.cn/gtqmffoaai.html

df -h;  du -sh *
来源：http://hz.guowangkeji.top/gtqimdoelu.html

[R62] 找最占空间的文件
来源：http://hz.chenlongwang.top/gtqxlszmce.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtjrtpjvhs.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gtxlpcffbt.html

free -h;  ps aux | grep nginx
来源：http://hz.c1oappe.top/gtdnuyvqjm.html

[R64] 结束进程
来源：http://hz.ywan-chungtsiang.top/gtqwvuafga.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gtrfbmresa.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtuwirsooz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtaredzwzc.html

[R66] 定时任务
来源：http://hz.sweek.top/gtrxmcnuor.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtaukultpd.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gthrxaysrl.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gttdihaxup.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gtmqqblthf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sysykeji.top/gtxhurwenu.html

[R69] 生成随机密码
来源：http://hz.cashguo.top/gtgtbldlcn.html

head -c 16 /dev/urandom | base64
来源：http://hz.fengsongda.top/gttrgvsgrs.html

[R70] 时间戳与互转
来源：http://hz.chenjidiqi.icu/gtpnauugrk.html

date +%s;  date -d @1700000000
来源：http://hz.zhijiandao.cn/gtldpilgei.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtpyimknym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.snrcjt.cn/gtvqtusixq.html

[R72] 等待端口就绪
来源：http://hz.sufxvd.cn/gtnbzsovgz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtubwgparz.html

[R73] 分割大日志
来源：http://hz.xuanzx.com/gtdokpcgdl.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtxeqluqnm.html

[R74] 批量重命名
来源：http://hz.yueranfly.top/gtytgvskno.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhengqikj.top/gtocfnnskd.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gtppjlsrcu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.feifeiyinyue.top/gtppetqyct.html

[R76] 使用临时文件
来源：http://hz.yj202588.top/gtcinpwrzv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtwybdfhak.html

[R77] 读取用户输入
来源：http://hz.yangfankeji.com/gtoudxisql.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtkczhbqzr.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtienrmlci.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gtptxcvfcu.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gthovwtloi.html


<!-- 参考信息 -->