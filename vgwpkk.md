代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gtccwanpzh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtcduvsbop.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtfhfenpxe.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtzlzrcmot.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtrehtbwfq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenzaomai.com/gtszugqtpt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yvedp.cn/gtfveuprdk.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gttcajzymo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gtciwdqxsn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.52xcode.cn/gtacbyezfp.html

[Q43] 标量子查询
来源：http://hz.sxryk.cn/gtrhhqxoga.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daria6918.cn/gtoemdmasn.html

[Q44] IN 子查询
来源：http://hz.aibaodan.cn/gthsfgiwbc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenjidiqi.icu/gtkqbqeqgy.html

[Q45] EXISTS 判断存在
来源：http://hz.guannengcc.top/gtutkecllu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtgxlkcxjc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnqzz.top/gtcvvjiwlg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtgiokkinq.html

[Q47] 与平均值比较
来源：http://hz.zhengqikj.top/gtmmweawjg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinghuilouyu.cn/gtprpwhkwz.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtqpvoeriz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hnqzz.top/gtanzygxko.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.andypj.xyz/gtqrzumeuu.html

[Q49] 更新单行
来源：http://hz.sxryk.cn/gtraiexnyo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtqxczppeu.html

[Q50] 批量更新
来源：http://hz.ivvv.top/gtyomtttva.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gttbtnljpy.html

[Q51] 用子查询更新
来源：http://hz.shuidangran.top/gtkqqmcees.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hysaishi.cn/gtxxsdhogh.html

[Q52] 删除指定行
来源：http://hz.tianlin.xyz/gtwciewaat.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtjcozfdgw.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtgrphzswd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gtdhkrijmi.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gthzoicxso.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258.top/gtxbgsjutl.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gtiscjaogz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yonumen.top/gtvsurlvri.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtvxuzuycl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aizwys.cn/gtxwllwfmx.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtqfwzqndz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhixingplan.top/gtawogmthg.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtzfxhawkb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gogol.net.cn/gtrvybhyws.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtdtghjnpj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgufenzy.top/gtjgklwvxp.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtaxpqvmci.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gtnnabdcdh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.havefunace.top/gtwbzfnbno.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtevcqcygc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.0kj1m.cn/gtawsuvmzl.html

[Q62] 分组占比
来源：http://hz.yuxming.cn/gtheyobjvf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtvmjtrgsu.html

[Q63] 开启事务
来源：http://hz.hfpthk.cn/gtfawrtahj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtanvsmohx.html

[Q64] 提交事务
来源：http://hz.zycfv.cn/gtltjjifhh.html

COMMIT;
来源：http://hz.c1oappe.top/gtlbiizjgr.html

[Q65] 回滚事务
来源：http://hz.c1oappe.top/gtaumdtwlm.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtlrflldnp.html

[Q66] 行锁查询
来源：http://hz.havefunace.top/gtlvtofqzm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zdqjudy.top/gttmvevpzc.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gtgamgnjfr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtqvagcndm.html

[Q68] 保存点
来源：http://hz.nanxuanxn.top/gtzboeyxoi.html

SAVEPOINT sp1;
来源：http://hz.9152youxi.cn/gtogkfwbyl.html

ROLLBACK TO sp1;
来源：http://hz.fzhhl.top/gtksszskjr.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gthjcvvxfr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yvedp.cn/gtpxpxkunc.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtjqaxkcku.html

ANALYZE TABLE users;
来源：http://hz.yvedp.cn/gtqjvawxcx.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtgkexikju.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinqigufen.top/gtaytmrwum.html

[Q72] 查看索引
来源：http://hz.gzhubu.top/gtogbnzgnt.html

SHOW INDEX FROM users;
来源：http://hz.xuanzx.com/gtysmtrcwt.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtlwzfqidy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tianlin.xyz/gtugzokziv.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtaqkpbrch.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtsvykwbbh.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtoahlxbzb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtmwdmaqet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hammf.cn/gttnklwnbj.html

[Q76] 按天统计
来源：http://hz.yangfankeji.com/gtxgszvztr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gtihlsmhlj.html

[Q77] 时间加减
来源：http://hz.gotoacloud.top/gtdbjshnkv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtyunpotkc.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gttapsszlg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenlongwang.top/gtyexsyadn.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtinngfpom.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shzxlz.cn/gtqtqwaenq.html

[Q80] 字符串截取
来源：http://hz.cashguo.top/gtpjcspmhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuetiantiany.cn/gtnisxkycx.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtepywthvj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtqcrngmrv.html

[Q82] 字符长度与字节长度
来源：http://hz.guowangkeji.top/gtlewdlvss.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtygkaktae.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gtiepeagbt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hammf.cn/gtfoxkgiad.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtfnjbsatb.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gttqvhikzb.html

[Q85] 数值取整
来源：http://hz.fengsongda.top/gtjkoiycea.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.316326.xyz/gtaascqnee.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gturihjrki.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gteipsawrp.html

[Q87] JSON 字段做条件
来源：http://hz.feifeiyinyue.top/gtybpyrhad.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sxryk.cn/gtqlovugaq.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gtlhfatzvl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.havefunace.top/gtyjkjtigs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtarevypnt.html

[Q89] 判断表是否存在
来源：http://hz.wangdashe.top/gtogjuihab.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yanxiufei.cn/gtnopicwwh.html

[Q90] 生成序号列
来源：http://hz.yj202588.top/gttgitcgza.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shuidangran.top/gtuqdypits.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbllrbjhl.html

R. Bash 专题
来源：http://hz.yuxming.cn/gthmueggma.html

================================================================================
来源：http://hz.tian-w.cn/gtjppydzme.html

[R01] shebang 与严格模式
来源：http://hz.ydjk.org.cn/gtsdbgbyvk.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gthqfocacp.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtycxlimlp.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtfxzdntot.html

name="Tom"; echo "$name"
来源：http://hz.fengsongda.top/gtmvtfkhau.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtngmwcski.html

readonly PI=3.14
来源：http://hz.hfpthk.cn/gtxkjubvgy.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtbrxbxkcq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtbtjtymkk.html

[R05] 参数默认值
来源：http://hz.zhongyouzk.top/gtoatktprw.html

name="${1:-default}"
来源：http://hz.c1oappe.top/gtzujhigdm.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtirrfficf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtelncqwdr.html

[R07] if 判断文件
来源：http://hz.birdmap.top/gttgmqnewd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnqzz.top/gtbpznlptn.html

[R08] 数值比较
来源：http://hz.dianchejie.cn/gtptywjlzl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gthicnrjjj.html

[R09] 字符串比较
来源：http://hz.jinqigfzy.top/gtqdfatsqq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtsjuobdia.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtrnfykloj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtpylrkdxz.html

[R11] case 多分支
来源：http://hz.meibo888.top/gtswzhdepn.html

case "$1" in
来源：http://hz.nanxuanxn.top/gttsqgfneh.html

start) echo "启动" ;;
来源：http://hz.yuanzhike.top/gtfdpicnmb.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtujmzitob.html

*)     echo "未知命令" ;;
来源：http://hz.wangdashe.top/gtsuiyembx.html

esac
来源：http://hz.xziqi.cn/gtpbmalpul.html

[R12] for 遍历文件
来源：http://hz.cashguo.top/gtkzzgplwg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtyaxgtauo.html

[R13] for 计数循环
来源：http://hz.iojbl.cn/gteiwnqqba.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tianlin.xyz/gtmahradwj.html

[R14] C 风格 for
来源：http://hz.pycfn.com/gtkhroaicu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtbrjkpvbj.html

[R15] while 逐行读文件
来源：http://hz.aibaodan.cn/gtooicvyoe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jlsjyb.cn/gtzhtzbvft.html

[R16] until 等待条件
来源：http://hz.jinghuilouyu.cn/gtprzzbkjn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtfmnlenrb.html

[R17] 数组定义与取值
来源：http://hz.jiagoushi.top/gtatjtolbi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtorplzzch.html

[R18] 遍历数组
来源：http://hz.daria6918.cn/gtprkxjiom.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxuanxn.top/gthgligrri.html

[R19] 数组长度
来源：http://hz.sysykeji.top/gtwbpqhgqy.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtebtrdkzp.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtnyeuvhmh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sufxvd.cn/gthvvzsnam.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtbbxoslbz.html

echo "${#s}"
来源：http://hz.wangshuangyany.cn/gtjfhxpdbx.html

[R22] 截取子串
来源：http://hz.tian-w.cn/gthncnehfu.html

echo "${s:0:5}"
来源：http://hz.dashuyun.cn/gttnwuvyem.html

[R23] 字符串替换
来源：http://hz.nanxinkj.top/gtarhlseth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtvpmvwgtj.html

[R24] 大小写转换
来源：http://hz.yanxiufei.cn/gtnktoootc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gthulymhyp.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuetiantiany.cn/gtrqfoyifi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gteozzqplr.html

[R26] 命令替换
来源：http://hz.tanke756.top/gtkrjjoifm.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gtowsbftnm.html

[R27] 算术展开
来源：http://hz.ydjk.org.cn/gtckcseuvr.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtoauvbtny.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtdflirnhw.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuanzx.com/gthjbqutdx.html

[R29] 定义函数
来源：http://hz.ydjk.org.cn/gtwzjjeoap.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtnbhqahfc.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtpazgmygn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtesodjsnd.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtkrryzeaa.html

f() { local x=1; echo "$x"; }
来源：http://hz.yongpay.top/gtbtxulplb.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtjhiyuney.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tian-w.cn/gteycrsrdi.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gtegfmcnir.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yvedp.cn/gtnroibkhj.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtxlmgcjlf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtrdlbhvaq.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtdoedrtzo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.0kj1m.cn/gtqnikrvyf.html

[R36] 并发执行多个任务
来源：http://hz.shuidangran.top/gtjssfnkmc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtmkujposq.html

[R37] 把输出赋给变量
来源：http://hz.daxiang520.top/gtewzzlsms.html

files=$(ls -1)
来源：http://hz.ppjwa.cn/gtfgzdyjvu.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gtdgxbawai.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tanke756.top/gtoavwzote.html

[R39] 重定向标准输出与错误
来源：http://hz.haohaochexian.top/gtcydnttoh.html

cmd > out.log 2>&1
来源：http://hz.fengsongda.top/gtldalugpv.html

[R40] 追加写日志
来源：http://hz.shzxlz.cn/gtwpgjputr.html

echo "log" >> out.log
来源：http://hz.wangshuangyany.cn/gtgczkpbuf.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gteapkmdpo.html

cmd >/dev/null 2>&1
来源：http://hz.316326.xyz/gtzbbhvrta.html

[R42] 输入重定向
来源：http://hz.sxryk.cn/gtbyckyxhc.html

wc -l < a.txt
来源：http://hz.cheryme.top/gtukxrkmzw.html

[R43] 按名字查找文件
来源：http://hz.cdnleiting.top/gtnzmrauoo.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gtexxglzez.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gttmpykjht.html

find . -mtime -7 -type f
来源：http://hz.feifeiyinyue.top/gtpbtjkijv.html

[R45] 批量删除
来源：http://hz.yuanzhike.top/gtnihgdszr.html

find . -name "*.tmp" -delete
来源：http://hz.feifeiyinyue.top/gtcthbtjls.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangtech.top/gtcgtztxms.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtyvqmorcd.html

[R47] sed 单行替换
来源：http://hz.gogol.net.cn/gtctkycncg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ybcxt.top/gtrumimeda.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gthcrmbrmb.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gthgmjwuch.html

[R49] awk 带条件
来源：http://hz.nanxinkj.top/gtxwjearan.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gtaaazxypt.html

[R50] awk 求和
来源：http://hz.wangdashe.top/gtfpqxuurh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gtcwoakyvo.html

[R51] 排序去重取前几
来源：http://hz.vqdsnc.cn/gtpbriwlla.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xylfe.cn/gtvotarvee.html

[R52] 统计行数
来源：http://hz.meibo888.top/gtjdzdahde.html

wc -l a.txt
来源：http://hz.yanxiufei.cn/gtvkoewzyl.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtgfxkjxnq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.mhx1999.top/gtffybaats.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gthoamflpd.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gtjgxxcwzi.html

[R55] 压缩与解压
来源：http://hz.yvedp.cn/gtxmeyidhq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinghuilouyu.cn/gtbwoxbpsy.html

[R56] 远程拷贝
来源：http://hz.xylfe.cn/gtqyyrrvpf.html

scp file user@host:/path/
来源：http://hz.haohaochexian.top/gturnytddu.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtppahnkvm.html

ssh user@host 'uptime'
来源：http://hz.iojbl.cn/gtxzcaipyn.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gtsostgvoa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gtviyovbdr.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtmwlsaxnp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnqzz.top/gthakyvuoq.html

[R60] 只看 HTTP 状态码
来源：http://hz.smart0.xyz/gtlsjfzvhi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shzxlz.cn/gtvqwtrsxy.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtfxzatags.html

df -h;  du -sh *
来源：http://hz.316326.xyz/gtbjwwzmcs.html

[R62] 找最占空间的文件
来源：http://hz.svipenyu.cn/gtwzrfdfby.html

du -ah . | sort -rh | head -10
来源：http://hz.xuanzx.com/gtwacoulsa.html

[R63] 内存与进程
来源：http://hz.iojbl.cn/gtkrkndmfi.html

free -h;  ps aux | grep nginx
来源：http://hz.haohaochexian.top/gtqleetvic.html

[R64] 结束进程
来源：http://hz.ehwqpu.com/gtncywerux.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtryacwiqw.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gtrwplczpe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhijiandao.cn/gtoosboywv.html

[R66] 定时任务
来源：http://hz.kuanghao11.cn/gterpszvoa.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtiwgybeor.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gtnolocsas.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtjxfngaoh.html

[R68] 计算文件校验值
来源：http://hz.yuanzhike.top/gtspycegeb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtxynkpgaf.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtdbcqrdzk.html

head -c 16 /dev/urandom | base64
来源：http://hz.andypj.xyz/gtqqzrvejt.html

[R70] 时间戳与互转
来源：http://hz.ywan-chungtsiang.top/gtlxoxgkwd.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gtajnzzhpc.html

[R71] 日期格式化
来源：http://hz.zycfv.cn/gtvbqndqyn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtfpmooubv.html

[R72] 等待端口就绪
来源：http://hz.wangshuangyany.cn/gtpmxynpyw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ppjwa.cn/gtfhzfozkn.html

[R73] 分割大日志
来源：http://hz.wangdashe.top/gtyadvjhdd.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtrkymzfsi.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gtpkkcqmgg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtyxkcsuhk.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtmkqplrpi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jlsjyb.cn/gtivarshpm.html

[R76] 使用临时文件
来源：http://hz.meibo888.top/gtsyvgslun.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtjdmwrqwy.html

[R77] 读取用户输入
来源：http://hz.yj202588.top/gtnteaejyk.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gtcmohacdv.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtvzvtmrss.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuxming.cn/gtbnspvahx.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtyzfdcspw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtqyjkcpvb.html

[R80] 查看脚本执行耗时
来源：http://hz.sweek.top/gtbkzdjhjr.html

time ./run.sh
来源：http://hz.gzhubu.top/gtbjueukvl.html

================================================================================
来源：http://hz.aibaodan.cn/gtiveefjnu.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtakxmtkyq.html

================================================================================
来源：http://hz.andypj.xyz/gtxdtuqybh.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gthfjfdfdn.html

#include <stdio.h>
来源：http://hz.tanke756.top/gtehselpsq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tanke756.top/gtlqxvaorj.html

[S02] C：变量与格式化输出
来源：http://hz.ydjk.org.cn/gtmbtrsqxr.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhixingplan.top/gtvrubsith.html

[S03] C：读入整数
来源：http://hz.ppjwa.cn/gtnywkrtkn.html

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtjxgtjlsv.html

[S04] C：字符串复制
来源：http://hz.fzhhl.top/gtpfcywkue.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shzxlz.cn/gtynbnsfiz.html

[S05] C：字符串长度
来源：http://hz.mhx1999.top/gtgffhtrnn.html

strlen(s)
来源：http://hz.chenlongwang.top/gtynaqifyc.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtlombdxdj.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangtech.top/gttlxdnupi.html

[S07] C：数组遍历求和
来源：http://hz.yj20258888.top/gtezsnnmqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtgrldfeuy.html

[S08] C：动态内存分配与释放
来源：http://hz.haohaochexian.top/gtcshgjhqb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gotoacloud.top/gtrktdjawx.html

[S09] C：结构体定义与初始化
来源：http://hz.sxryk.cn/gtneqxawkn.html


<!-- 参考信息 -->