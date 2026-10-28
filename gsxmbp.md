代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtusewuybu.html

[Q54] 清空表
来源：http://hz.gotoacloud.top/gtzuqzqbpg.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtksxxvxwo.html

[Q55] 排名（并列占位）
来源：http://hz.316326.xyz/gtnqyfabrc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhiwuduotai.top/gtrxjoevop.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jlsjyb.cn/gtmyolicyg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtneakbbby.html

[Q57] 行号
来源：http://hz.zhiwuduotai.top/gtvsmyvtno.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pengpengdd.cyou/gtcffnpaqe.html

[Q58] 累计求和
来源：http://hz.yvedp.cn/gtgofvvvpj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtovdfxbnf.html

[Q59] 分组内累计
来源：http://hz.cucudq.cn/gtqbzxqbvl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gtfzuxlfin.html

[Q60] 取上一行 / 下一行
来源：http://hz.cashguo.top/gthufjmssn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.smart0.xyz/gtayhttxkq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtujsbwtvt.html

[Q61] 移动平均
来源：http://hz.mhx1999.top/gtlujjncdl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tian-w.cn/gtbhscgdgf.html

[Q62] 分组占比
来源：http://hz.vqdsnc.cn/gtygqlbnwn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtfmkhxflr.html

[Q63] 开启事务
来源：http://hz.jqgufenzy.top/gtvoojitrl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtzfgsvgjk.html

[Q64] 提交事务
来源：http://hz.aibaodan.cn/gtbpplfegf.html

COMMIT;
来源：http://hz.xingfuxueyuan.xyz/gtfilqabaf.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtkjzyahuq.html

ROLLBACK;
来源：http://hz.xziqi.cn/gtewfywjlt.html

[Q66] 行锁查询
来源：http://hz.quarkkingdee.top/gthbtgamfn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ehwqpu.com/gtcfvenbhx.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtcfxkwtoc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gtzhcimayb.html

[Q68] 保存点
来源：http://hz.c1oappe.top/gtufptfrby.html

SAVEPOINT sp1;
来源：http://hz.shzxlz.cn/gtdptdrqyj.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtdysmkshp.html

[Q69] 查看执行计划
来源：http://hz.mhx1999.top/gtpdtazpyo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cashguo.top/gtsaofpiyy.html

[Q70] 更新统计信息
来源：http://hz.zhengqikj.top/gtcocsvlag.html

ANALYZE TABLE users;
来源：http://hz.gogol.net.cn/gtetzwbtez.html

[Q71] 查看建表语句
来源：http://hz.hysaishi.cn/gtrmfwmokq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.iojbl.cn/gtlxmsqhdz.html

[Q72] 查看索引
来源：http://hz.sweek.top/gtluogvysx.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gttjxlglyl.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gttobbukqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gtxoayyyvx.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gtigyrbvww.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtlwtuyydj.html

[Q75] 日期格式化
来源：http://hz.guowangkeji.top/gtwziqkbmh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtrmkurjyl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.0kj1m.cn/gtkujydjfz.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtpvudlfjp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gtrigfkeco.html

[Q77] 时间加减
来源：http://hz.yvedp.cn/gtpluqvbqo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.svipenyu.cn/gtvwsjxdet.html

[Q78] 当前时间
来源：http://hz.xziqi.cn/gtrfxrcowy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.316326.xyz/gtzxcianbu.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtinxrqejc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gthhrepuad.html

[Q80] 字符串截取
来源：http://hz.cucudq.cn/gtdhyldeia.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtgxmewilq.html

[Q81] 字符串替换
来源：http://hz.gogol.net.cn/gtsnalxffu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shangyingyoupin.top/gtypiqmjtv.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtufbvqvsw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtvmxdegoy.html

[Q83] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtqegalsny.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtrwntisph.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtxhmoqxni.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gtunozdsle.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtnsroxihu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgufenzy.top/gtkocsjvkh.html

[Q86] 读取 JSON 字段
来源：http://hz.jiagoushi.top/gtumexlkdh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgufenzy.top/gtcpgzgvky.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gtdebemxmf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sxryk.cn/gtmepibekw.html

[Q88] 行转列（条件聚合）
来源：http://hz.yueranfly.top/gtivhggmqo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gtefndmymc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtycvsgxmr.html

[Q89] 判断表是否存在
来源：http://hz.xingfuxueyuan.xyz/gtaxmlrmbh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhaomingkeji.xyz/gtiacqofso.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gtpmajvtdd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xingfuxueyuan.xyz/gtwfwpjngj.html

================================================================================
来源：http://hz.redwolf501.top/gtlntcbaqr.html

R. Bash 专题
来源：http://hz.jinqigfzy.top/gtukondcpd.html

================================================================================
来源：http://hz.svipenyu.cn/gtcgqrsite.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtdeewimwi.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtiznhqyhm.html

set -euo pipefail
来源：http://hz.svipenyu.cn/gtbpuldsmi.html

[R02] 变量赋值与使用
来源：http://hz.gogol.net.cn/gtjjnwhwfu.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gthxhbanqm.html

[R03] 只读变量
来源：http://hz.yuxming.cn/gtievczyqw.html

readonly PI=3.14
来源：http://hz.yj202588.top/gtifslyzeu.html

[R04] 位置参数
来源：http://hz.snrcjt.cn/gtxibmiqdy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gtcobqfsge.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtcuymtpor.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtrvsicwjn.html

[R06] 判断命令是否存在
来源：http://hz.dashuyun.cn/gtighkodax.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtpohsnswg.html

[R07] if 判断文件
来源：http://hz.fengsongda.top/gtvkyvzjyy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fzhhl.top/gtoqjsbltp.html

[R08] 数值比较
来源：http://hz.zhongyouzk.top/gtqsyugmux.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gtuzbjngxv.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtbfavfwqt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtnwmrsncw.html

[R10] 正则匹配
来源：http://hz.daria6918.cn/gtzxhutvfc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.snrcjt.cn/gtksbtceqt.html

[R11] case 多分支
来源：http://hz.dianchejie.cn/gtneaghadg.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtkdbtgsze.html

start) echo "启动" ;;
来源：http://hz.tianlin.xyz/gttowerxgx.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtynknnnvw.html

*)     echo "未知命令" ;;
来源：http://hz.zdqjudy.top/gtuqrinvsp.html

esac
来源：http://hz.hongshengwenyu.top/gtlporknvy.html

[R12] for 遍历文件
来源：http://hz.dashuyun.cn/gtafqjmgcy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xylfe.cn/gtmqvqggxh.html

[R13] for 计数循环
来源：http://hz.smart0.xyz/gtyxnlabbs.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigufen.top/gtyukllusy.html

[R14] C 风格 for
来源：http://hz.ywan-chungtsiang.top/gtsisxqtaq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtauytfdhk.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtoghdmuqg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtxhtcgokl.html

[R16] until 等待条件
来源：http://hz.yuxming.cn/gtwiqmjvzh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hywenlv.cn/gtwqgdeeja.html

[R17] 数组定义与取值
来源：http://hz.xuetiantiany.cn/gtbuglkbbp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtcczhvtjc.html

[R18] 遍历数组
来源：http://hz.gogol.net.cn/gtfnfmncqm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhixingplan.top/gtngysobix.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtujilsxma.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtonucthge.html

[R20] 关联数组（字典）
来源：http://hz.yueranfly.top/gtsalrazai.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gtsxwntmuo.html

[R21] 字符串长度
来源：http://hz.ydjk.org.cn/gtgaovtdqz.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtrpybvsaz.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gtpgipojiq.html

echo "${s:0:5}"
来源：http://hz.yuxming.cn/gtvgznrwlt.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtpfkjevsm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtxiykofyc.html

[R24] 大小写转换
来源：http://hz.jiagoushi.top/gtyljcmqrs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guannengcc.top/gtejxvyrbu.html

[R25] 去后缀 / 去前缀
来源：http://hz.jiagoushi.top/gtskgvjzpy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtcwmjuhvw.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gtlywurhdj.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtboitlmwm.html

[R27] 算术展开
来源：http://hz.hammf.cn/gthdrjbpyy.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtvgcvrtvk.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtjlsnhoka.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtegzoewka.html

[R29] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtcqiuecpx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gthetejjxv.html

[R30] 函数返回状态码
来源：http://hz.dianchejie.cn/gtauuqsyqp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtjstpnxuh.html

[R31] 局部变量
来源：http://hz.iojbl.cn/gtqpzysiug.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtxtzkjcdz.html

[R32] 参数个数校验
来源：http://hz.ivvv.top/gtxjceddfb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtrimwsbka.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtqvyfsadb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtkuihqlhk.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gtxklozofm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtofvxqunv.html

[R35] 后台执行并等待
来源：http://hz.aibaodan.cn/gtxlwvexef.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtzdhaeovb.html

[R36] 并发执行多个任务
来源：http://hz.hywenlv.cn/gtpjukcegk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuetiantiany.cn/gtzeefeick.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangtech.top/gtdhuwssca.html

files=$(ls -1)
来源：http://hz.tian-w.cn/gtvmhonvtr.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gttjvhpbrm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigfzy.top/gtshypolvq.html

[R39] 重定向标准输出与错误
来源：http://hz.zhoulong.xyz/gtiujvllpk.html

cmd > out.log 2>&1
来源：http://hz.zhijiandao.cn/gtvsvhdexj.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtnyvjjqxx.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtbivwuxcq.html

[R41] 丢弃输出
来源：http://hz.yangfankeji.com/gtbuxtqhxe.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtwzuxywbp.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtnldlxmnt.html

wc -l < a.txt
来源：http://hz.jqgufenzy.top/gtsxpknxnj.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtvwfcyndq.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtyzqijrrs.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtsboxoxcz.html

find . -mtime -7 -type f
来源：http://hz.snrcjt.cn/gtlxjqmnrv.html

[R45] 批量删除
来源：http://hz.gzhubu.top/gtjuyqnzgt.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigufen.top/gtshjxhqfl.html

[R46] 递归替换文件内容
来源：http://hz.feifeiyinyue.top/gtfsickfaz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jyoumei.cn/gtgkgyxaqg.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtusxzjvcd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtxxhqusyo.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtdpqkowdr.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gtbjjkwzea.html

[R49] awk 带条件
来源：http://hz.yj202588.top/gtczymdali.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.redwolf501.top/gtxawwgupx.html

[R50] awk 求和
来源：http://hz.hnxiangtu.top/gtmaidqlho.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hywenlv.cn/gtnoqtdjuy.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtmdrjjpyb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtzrkujyrp.html

[R52] 统计行数
来源：http://hz.xuanzx.com/gtthsbkozd.html

wc -l a.txt
来源：http://hz.gaohongyu789.top/gtwdrqugff.html

[R53] 查看文件头与实时尾
来源：http://hz.pengpengdd.cyou/gtfualjvwc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sysykeji.top/gtmkqpfbtf.html

[R54] 比较两个文件
来源：http://hz.nwbrower.top/gtfxbkrrhq.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtubuytulc.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtyfuydenk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shzxlz.cn/gtjdfevmnv.html

[R56] 远程拷贝
来源：http://hz.wangshuangyany.cn/gtfqyjjoua.html

scp file user@host:/path/
来源：http://hz.tianlin.xyz/gtakbzduge.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtpvnmhdem.html

ssh user@host 'uptime'
来源：http://hz.xuanzx.com/gtwzcaarec.html

[R58] 下载文件
来源：http://hz.gogol.net.cn/gtzchyjosg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtixfrmadm.html

[R59] 发 POST JSON
来源：http://hz.sweek.top/gttekgemrp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtcsrzyamn.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtzzwtwufv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangshuangyany.cn/gtymtlkpvn.html

[R61] 磁盘占用
来源：http://hz.hnqzz.top/gtwgbzwaxo.html

df -h;  du -sh *
来源：http://hz.aibaodan.cn/gtsigzpuqh.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gtbgyoqwih.html

du -ah . | sort -rh | head -10
来源：http://hz.c1oappe.top/gtqsprhzyh.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gttdehtaol.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtzfaizdbg.html

[R64] 结束进程
来源：http://hz.xuanzx.com/gtibqiwbam.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj202588.top/gtxanxhbxa.html

[R65] 查看端口占用
来源：http://hz.daria6918.cn/gtqhsimfjz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtrzrwgyyi.html

[R66] 定时任务
来源：http://hz.zhoulong.xyz/gtfirfflpy.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtrhwnqwtj.html

[R67] 生成随机十六进制串
来源：http://hz.xinyue.icu/gtynadiunv.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gtiudpgpfc.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtgqktzzce.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sysykeji.top/gtvqsluhua.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtmqmdyfpt.html

head -c 16 /dev/urandom | base64
来源：http://hz.jiagoushi.top/gtjeekfemb.html

[R70] 时间戳与互转
来源：http://hz.aibaodan.cn/gtyqatunhp.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gtqfrwzsvb.html

[R71] 日期格式化
来源：http://hz.chenlongwang.top/gtshynbpfv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtjzsfizgn.html

[R72] 等待端口就绪
来源：http://hz.yuxming.cn/gtsvmlxfmn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dashuyun.cn/gtyxedssxr.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtcjjdaare.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtztmrffpj.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtoiitbpxl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangshuangyany.cn/gtfjghdbpm.html

[R75] 导出环境变量
来源：http://hz.sufxvd.cn/gtsbiylswh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guannengcc.top/gthooovric.html

[R76] 使用临时文件
来源：http://hz.ydjk.org.cn/gtppjdyomg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtapdhybjz.html

[R77] 读取用户输入
来源：http://hz.tanke756.top/gtlhftjdkk.html

read -rp "请输入: " ans
来源：http://hz.hysaishi.cn/gtpwakrdal.html

[R78] 交互式菜单
来源：http://hz.yvedp.cn/gtavllcjhn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtzlbkmxer.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtnkubupnf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgufenzy.top/gtzcxtpqte.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtxmzaxjbo.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtzobeigjd.html

================================================================================
来源：http://hz.chenlongwang.top/gtapmuokph.html

S. C / C++ 专题
来源：http://hz.ywan-chungtsiang.top/gtrkzvwbgm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjedbpbpe.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gtcktyoogm.html

#include <stdio.h>
来源：http://hz.tanke756.top/gteghupray.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.meibo888.top/gtztnwyxnw.html

[S02] C：变量与格式化输出
来源：http://hz.snrcjt.cn/gttdvqruyo.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gthlhbkpae.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gtqgqgwhjh.html

int x; scanf("%d", &x);
来源：http://hz.xuetiantiany.cn/gtmvpqeqrq.html

[S04] C：字符串复制
来源：http://hz.sufxvd.cn/gtbiuilnbr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtgexnrkkf.html

[S05] C：字符串长度
来源：http://hz.yuxming.cn/gtlclcdgiw.html

strlen(s)
来源：http://hz.zhongyouzk.top/gtqtafptyz.html

[S06] C：字符串比较
来源：http://hz.aizwys.cn/gtiropogth.html

strcmp(a, b) == 0
来源：http://hz.gzhubu.top/gtzgtlqsln.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtxuobiijj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydjk.org.cn/gtmtttgenn.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgufenzy.top/gtiafnrcag.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jyoumei.cn/gtebgfpaqg.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gtdqqdziaj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daria6918.cn/gtoxhzqtmp.html

[S10] C：指针与解引用
来源：http://hz.vqdsnc.cn/gttaasrfhq.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtxcqfspsm.html

[S11] C：逐行读文件
来源：http://hz.cucudq.cn/gtruorjmnh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gotoacloud.top/gtupwjzahc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhongyouzk.top/gtfbiyagwo.html

fclose(f);
来源：http://hz.hammf.cn/gtklibinql.html

[S12] C：写文件
来源：http://hz.gaohongyu789.top/gtzfqsmmit.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtqjncyxrh.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtzdfagzxw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xingfuxueyuan.xyz/gtqkwmvumf.html

[S14] C：枚举
来源：http://hz.quarkkingdee.top/gtmmsenjub.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtuildmhfs.html

[S15] C：类型转换
来源：http://hz.shuidangran.top/gtevtfpoun.html

(double) a / b
来源：http://hz.hfpthk.cn/gtrmubictb.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtbwnpqwir.html

x |= (1 << 3);
来源：http://hz.iojbl.cn/gtuycjoiuh.html

[S17] C：安全拼接字符串
来源：http://hz.jlsjyb.cn/gtuccipjwm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangshuangyany.cn/gtgtqguxxy.html

[S18] C：命令行参数
来源：http://hz.shzxlz.cn/gtdepbeiln.html

int main(int argc, char **argv)
来源：http://hz.yueranfly.top/gtkgyrmkft.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gtubpvfdox.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtwesxatoz.html

[S20] C：二分查找
来源：http://hz.zhijiandao.cn/gtvromgmnu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtyppzfbac.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtapmfydxe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhoulong.xyz/gtufdbnycu.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtyyyrqgex.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hammf.cn/gtltaqwfzm.html

[S23] C：随机数
来源：http://hz.nanxinkj.top/gtsutpcaal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gotoacloud.top/gtcrbapcoo.html

[S24] C：获取本地时间
来源：http://hz.zhaomingkeji.xyz/gteshyafhr.html


<!-- 参考信息 -->