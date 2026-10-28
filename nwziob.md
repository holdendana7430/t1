代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yanxiufei.cn/gtlnellxra.html

[Q32] 分组拼接字符串
来源：http://hz.fzhhl.top/gtoetwswzw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtelfmesgf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtrthusxoz.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtiayrcxgq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shuidangran.top/gtryurdedr.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtsxelhhhi.html

SELECT * FROM (
来源：http://hz.chenlongwang.top/gtsgdsctgd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.feifeiyinyue.top/gtaskrundd.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtjekzpwrq.html

[Q35] 内连接
来源：http://hz.bjfxy.top/gtldzxeadg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtdnvigwsa.html

[Q36] 左连接
来源：http://hz.chenzaomai.com/gtnymryxuc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtmapfcnhh.html

[Q37] 右连接
来源：http://hz.ivvv.top/gtgcfbtwxj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.redwolf501.top/gtxtsbfgja.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tianlin.xyz/gtihfvbbtj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhongyouzk.top/gtqnumdosf.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtztgisyws.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuanzx.com/gtoywgujjf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtvefqarpw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.birdmap.top/gtvhgxbskt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj202588.top/gtmtjpjvpe.html

[Q41] 多表连接
来源：http://hz.zhijiandao.cn/gtqgfydbdu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtsmiynfle.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtbwpojucs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zdqjudy.top/gtaozzdxre.html

[Q42] 连接条件附加过滤
来源：http://hz.ydjk.org.cn/gtajutvtga.html

SELECT u.name, o.amount FROM users u
来源：http://hz.guannengcc.top/gtgyexofno.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtyczuobpq.html

[Q43] 标量子查询
来源：http://hz.guowangkeji.top/gtzeikibul.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.iojbl.cn/gtenpuykwh.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gtotzwrqcq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gotoacloud.top/gtfpeksgsu.html

[Q45] EXISTS 判断存在
来源：http://hz.shangyingyoupin.top/gtnchfnisi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtzzarmkkw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gttoidepgy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtmhxfduxc.html

[Q47] 与平均值比较
来源：http://hz.daria6918.cn/gtxyvtuqoc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gtemxpzvyk.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtsxicjtrs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guannengcc.top/gtjprhiskb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gtqggwckzx.html

[Q49] 更新单行
来源：http://hz.zhixingplan.top/gtqtvndhft.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gotoacloud.top/gtvwzoabhj.html

[Q50] 批量更新
来源：http://hz.shzxlz.cn/gtfcbwtvpq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sufxvd.cn/gtzyckevrq.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtfberfodu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jianghu66.top/gthlwsibyj.html

[Q52] 删除指定行
来源：http://hz.jinghuilouyu.cn/gtiezxxbda.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gttwdabvlg.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtnifmrpsi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.52xcode.cn/gtnplejiop.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtdwfyyfdo.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtvatigurf.html

[Q55] 排名（并列占位）
来源：http://hz.tanke756.top/gtxakrdjxv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtyhurvouy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtrutvkwya.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shzxlz.cn/gtlhqsjfee.html

[Q57] 行号
来源：http://hz.yongpay.top/gtwbebvgrl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.iojbl.cn/gtzewxvrcy.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtfxbyifpz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtapxnzohp.html

[Q59] 分组内累计
来源：http://hz.ydzc1.top/gtfkykqzsd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gthkhfyonm.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtrowblgbi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtcokvbmeu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtpeymedmb.html

[Q61] 移动平均
来源：http://hz.jyoumei.cn/gtewqudebs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gthctfaoam.html

[Q62] 分组占比
来源：http://hz.birdmap.top/gtthulqysk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtzseekpku.html

[Q63] 开启事务
来源：http://hz.yvedp.cn/gtisqlengz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydjk.org.cn/gtndofugin.html

[Q64] 提交事务
来源：http://hz.bjfxy.top/gtadaieyys.html

COMMIT;
来源：http://hz.9152youxi.cn/gtqevnawmn.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtbfxbmggw.html

ROLLBACK;
来源：http://hz.haohaochexian.top/gtaphozxsj.html

[Q66] 行锁查询
来源：http://hz.yuanzhike.top/gtjhvhrzuz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fzhhl.top/gtwomkygvp.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtsgabhzpd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guannengcc.top/gteeeossfo.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtdjyndhjc.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtqfxaxwao.html

ROLLBACK TO sp1;
来源：http://hz.sufxvd.cn/gtubfvfgtg.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtfzxsfngz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xylfe.cn/gtcaaeaeck.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gthfrsqkuo.html

ANALYZE TABLE users;
来源：http://hz.jinqigufen.top/gtyxtmngne.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtahzqeodd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gtgdocpqsk.html

[Q72] 查看索引
来源：http://hz.nanxinkj.top/gtuogqyund.html

SHOW INDEX FROM users;
来源：http://hz.ybcxt.top/gturtrqluk.html

[Q73] 查看表状态
来源：http://hz.smart0.xyz/gtarzbsdzx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtotnfmvxp.html

[Q74] 强制使用索引
来源：http://hz.cqqwz.cn/gtsyflfies.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.9152youxi.cn/gtndpsejaa.html

[Q75] 日期格式化
来源：http://hz.havefunace.top/gtjmqmoooa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jyoumei.cn/gtmjbgillv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenlongwang.top/gtxaeizuza.html

[Q76] 按天统计
来源：http://hz.cucudq.cn/gtbxpgcikj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zdqjudy.top/gtyafkkbky.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtxxqrtbeu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aibaodan.cn/gtrudzkqrp.html

[Q78] 当前时间
来源：http://hz.ppjwa.cn/gtznbvoieg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sweek.top/gtdnpgnzlu.html

[Q79] 字符串拼接
来源：http://hz.wangshuangyany.cn/gtpptffijc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuanzx.com/gtrrkuncqn.html

[Q80] 字符串截取
来源：http://hz.yuanzhike.top/gtmmynelvq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shangyingyoupin.top/gtnefkxasi.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtfdmkvyxr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinghuilouyu.cn/gtjptycpop.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gtijmaoyzy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nwbrower.top/gtvktrgxvq.html

[Q83] 大小写转换
来源：http://hz.sysykeji.top/gtcbjuyyup.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.snrcjt.cn/gtdfwlsaib.html

[Q84] 去除首尾空格
来源：http://hz.bjfxy.top/gtjhrcwnvz.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtnqihmitl.html

[Q85] 数值取整
来源：http://hz.c1oappe.top/gtbkzjwrwc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hongshengwenyu.top/gtgzlbfdme.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtiniswxms.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shangyingyoupin.top/gtkukrlcty.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtymisskwk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gogol.net.cn/gttvmgteka.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtaegrjyxx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.snrcjt.cn/gtcxxncgyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guowangkeji.top/gtcxyqfnon.html

[Q89] 判断表是否存在
来源：http://hz.cdnleiting.top/gtmeqpwalx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhaomingkeji.xyz/gtyoqvaqhz.html

[Q90] 生成序号列
来源：http://hz.tian-w.cn/gteuhtvlld.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tianlin.xyz/gtvmhryqub.html

================================================================================
来源：http://hz.gotoacloud.top/gtlifnttgy.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gthubzjyvr.html

================================================================================
来源：http://hz.yueranfly.top/gtigyxjnfz.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtojoiilfu.html

#!/usr/bin/env bash
来源：http://hz.yuanzhike.top/gtslkxngkk.html

set -euo pipefail
来源：http://hz.9152youxi.cn/gtsnobzetd.html

[R02] 变量赋值与使用
来源：http://hz.vqdsnc.cn/gtldtapwjl.html

name="Tom"; echo "$name"
来源：http://hz.ehwqpu.com/gtobwlkono.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gtyfkyuzda.html

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gtlgrqicgh.html

[R04] 位置参数
来源：http://hz.yuxming.cn/gtwacnvscv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtuuoozysn.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gtkcbcwbsm.html

name="${1:-default}"
来源：http://hz.pengpengdd.cyou/gtxnmohbcz.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtoygjtldv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtzdsvcfel.html

[R07] if 判断文件
来源：http://hz.zhengqikj.top/gtelusmpbm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yongpay.top/gtcercuswf.html

[R08] 数值比较
来源：http://hz.birdmap.top/gtfprilwds.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hammf.cn/gtadxcnfjs.html

[R09] 字符串比较
来源：http://hz.bjfxy.top/gtwberhsnd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtlujkknrs.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtufqvzgfk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ydjk.org.cn/gtlfmnseuo.html

[R11] case 多分支
来源：http://hz.meibo888.top/gtkumrwkva.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtgprmzfom.html

start) echo "启动" ;;
来源：http://hz.zhiwuduotai.top/gtgbvgqhbv.html

stop)  echo "停止" ;;
来源：http://hz.nanxuanxn.top/gthafkxpur.html

*)     echo "未知命令" ;;
来源：http://hz.xingfuxueyuan.xyz/gtoeeioyso.html

esac
来源：http://hz.jinyuanbaomall.cn/gtukgmgqfc.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtxnyuxyup.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnxiangtu.top/gtgnujzowa.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtsabjviue.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgfzy.top/gtgzmbtzcr.html

[R14] C 风格 for
来源：http://hz.birdmap.top/gtuapoltov.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.mhx1999.top/gtdirxqbbw.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gtuvdnklcc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangkeji.top/gtwcahglvl.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gtbbwohuyh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtunonycck.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtsdnauntt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.smart0.xyz/gtdhuormbw.html

[R18] 遍历数组
来源：http://hz.meibo888.top/gtstczcjog.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.52xcode.cn/gthpuqiwsf.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtwsivvspq.html

echo "${#arr[@]}"
来源：http://hz.yj202588.top/gtfgvlzemn.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtgnejagax.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aizwys.cn/gthvlstida.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gthlbxfkty.html

echo "${#s}"
来源：http://hz.ppjwa.cn/gtsbrfruth.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gtmlguvbxz.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtatlsynpm.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtrejocgao.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cqqwz.cn/gtjmbwunta.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtogzvgqmq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gtxwhsonba.html

[R25] 去后缀 / 去前缀
来源：http://hz.ywan-chungtsiang.top/gtsbypbjue.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xylfe.cn/gtdxcwyozn.html

[R26] 命令替换
来源：http://hz.xuetiantiany.cn/gtzogsdlmi.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtylwifkbf.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtbqhlprdz.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtglegciyx.html

[R28] 浮点运算
来源：http://hz.daria6918.cn/gtdpgvwsri.html

echo "scale=2; 10/3" | bc
来源：http://hz.havefunace.top/gtwrqvxzkl.html

[R29] 定义函数
来源：http://hz.gaohongyu789.top/gtqvwjeiqu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtbqfnfqwf.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtsigcjewt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gtlkvkpbtu.html

[R31] 局部变量
来源：http://hz.shanyushiyangtech.top/gtpszjhgnx.html

f() { local x=1; echo "$x"; }
来源：http://hz.jianghu66.top/gtyvfphqqk.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gttlqzyqlz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtmbrosbdi.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtpdfibfnx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xinyue.icu/gtegtydoju.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtabqseskd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtajetvhvi.html

[R35] 后台执行并等待
来源：http://hz.316326.xyz/gtwfsiezjo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtjuinkqeo.html

[R36] 并发执行多个任务
来源：http://hz.9152youxi.cn/gtwpvqdhla.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jianghu66.top/gtlxvakeso.html

[R37] 把输出赋给变量
来源：http://hz.svipenyu.cn/gtvxiskdpu.html

files=$(ls -1)
来源：http://hz.snrcjt.cn/gtitzjldfk.html

[R38] 管道串联
来源：http://hz.jyoumei.cn/gtkppggnta.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jiagoushi.top/gtewiesdsb.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtuhcjtbeh.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gtsnwcfwbb.html

[R40] 追加写日志
来源：http://hz.wangshuangyany.cn/gtyogiciuj.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtrdsezcld.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtbimtqhst.html

cmd >/dev/null 2>&1
来源：http://hz.gotoacloud.top/gtzatolacy.html

[R42] 输入重定向
来源：http://hz.dashuyun.cn/gttafooznk.html

wc -l < a.txt
来源：http://hz.sweek.top/gtggspqbnw.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtakfbrbsz.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtmdvpawbe.html

[R44] 按修改时间查找
来源：http://hz.xuetiantiany.cn/gtliwducwu.html

find . -mtime -7 -type f
来源：http://hz.nanxuanxn.top/gtuoqfgzln.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtezpjtrtu.html

find . -name "*.tmp" -delete
来源：http://hz.ydjk.org.cn/gtlpekeave.html

[R46] 递归替换文件内容
来源：http://hz.pengpengdd.cyou/gtcvotiqyb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.meibo888.top/gtigegqhrw.html

[R47] sed 单行替换
来源：http://hz.sysykeji.top/gtdfoiunce.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtqfojubil.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtuujvioad.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gtzuflvmay.html

[R49] awk 带条件
来源：http://hz.sxryk.cn/gtnjhrhulm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gzhubu.top/gthdqqxqfp.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtkznktpjr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtlzclgquq.html

[R51] 排序去重取前几
来源：http://hz.yuxming.cn/gtjvioxfet.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gttjoqpulr.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtovzcrazk.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtdvrozsai.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtpcywdlye.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yangfankeji.com/gthyqlyaph.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtcowhmqiz.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gtsxghktes.html

[R55] 压缩与解压
来源：http://hz.sysykeji.top/gtgpfwrcbg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gtlxklzypq.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtholthclv.html

scp file user@host:/path/
来源：http://hz.ybcxt.top/gtxnlnaeqh.html

[R57] 远程执行命令
来源：http://hz.wangdashe.top/gtfalomzqg.html

ssh user@host 'uptime'
来源：http://hz.ivvv.top/gtnhkvaboy.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gtjssxlbpp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuanzx.com/gtaegyxdit.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtiwzpppuc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sxryk.cn/gtbbpntull.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtbtugtaot.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nwbrower.top/gtnyngiusa.html

[R61] 磁盘占用
来源：http://hz.kuanghao11.cn/gtiimvfcqg.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gtiqrnvnxb.html

[R62] 找最占空间的文件
来源：http://hz.ydzc1.top/gtpvjmbxye.html

du -ah . | sort -rh | head -10
来源：http://hz.zhongyouzk.top/gtqinunbqr.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtnapzplkh.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtylqncjgz.html

[R64] 结束进程
来源：http://hz.sweek.top/gtdrqskqpm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtevdshwiq.html

[R65] 查看端口占用
来源：http://hz.shuidangran.top/gtryqelksg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gthsssyvyr.html

[R66] 定时任务
来源：http://hz.sxryk.cn/gtshdxxexa.html

crontab -e;  crontab -l
来源：http://hz.hammf.cn/gtdstsydbz.html

[R67] 生成随机十六进制串
来源：http://hz.cqqwz.cn/gtbuqhmvuo.html

openssl rand -hex 16
来源：http://hz.jinqigfzy.top/gtgqoxrdoa.html

[R68] 计算文件校验值
来源：http://hz.jiagoushi.top/gtkzjulavu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zycfv.cn/gthfjejpva.html

[R69] 生成随机密码
来源：http://hz.hywenlv.cn/gtvpnttzhx.html

head -c 16 /dev/urandom | base64
来源：http://hz.yonumen.top/gteffsyyig.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtwlmxgonf.html

date +%s;  date -d @1700000000
来源：http://hz.jlsjyb.cn/gtbcuxedmu.html

[R71] 日期格式化
来源：http://hz.daria6918.cn/gtimvfldwb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtpopdskkl.html

[R72] 等待端口就绪
来源：http://hz.zhiwuduotai.top/gttfwjjrdu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dianchejie.cn/gtbxnugsji.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtrvsacnav.html

split -l 1000 big.log part_
来源：http://hz.vqdsnc.cn/gtejtmqenl.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gteymaxwvs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhoulong.xyz/gtxznpglrr.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtbozrqumu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtpjogamqx.html

[R76] 使用临时文件
来源：http://hz.xinyue.icu/gtyiijseeo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtgcdfpwea.html

[R77] 读取用户输入
来源：http://hz.0kj1m.cn/gtdntqbswo.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtejmyauqi.html

[R78] 交互式菜单
来源：http://hz.zhixingplan.top/gtrueddngp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cdnleiting.top/gtpwdnryun.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gttiyomams.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtknfalokb.html

[R80] 查看脚本执行耗时
来源：http://hz.gaohongyu789.top/gtxuhsvspo.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtefbqynjm.html

================================================================================
来源：http://hz.shuidangran.top/gtcuwvpyhm.html


<!-- 参考信息 -->