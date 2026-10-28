代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gtwtghlral.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtmpgbhhzk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gtaweotpsw.html

[Q53] 按条件删除
来源：http://hz.mhx1999.top/gtisqhrxpg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtoqcpinri.html

[Q54] 清空表
来源：http://hz.shzxlz.cn/gtxgxplkvu.html

TRUNCATE TABLE logs;
来源：http://hz.zdqjudy.top/gtggcpkquu.html

[Q55] 排名（并列占位）
来源：http://hz.meibo888.top/gtbhazdoud.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnqzz.top/gtwwmidolq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenjidiqi.icu/gtzwkklpty.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhiwuduotai.top/gthrbhmmub.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtqvfvjvfc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gtabfealut.html

[Q58] 累计求和
来源：http://hz.dianchejie.cn/gtwhlcnhjc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtsepwbnzt.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtusqobqrl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtpnwmznli.html

[Q60] 取上一行 / 下一行
来源：http://hz.cucudq.cn/gtwkirgfmn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jiagoushi.top/gtpneujogx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aibaodan.cn/gtswanftxx.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gtccgbfffs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtaagygsmz.html

[Q62] 分组占比
来源：http://hz.xingfuxueyuan.xyz/gtdsfvsliw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtdmijddux.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gttetcbwrq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtairbvenr.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtuxykklvz.html

COMMIT;
来源：http://hz.dianchejie.cn/gtuzrmrbmr.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtmykdnnew.html

ROLLBACK;
来源：http://hz.yanxiufei.cn/gtkhsygjgq.html

[Q66] 行锁查询
来源：http://hz.dashuyun.cn/gtbnuzqwhj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yanxiufei.cn/gtpvamtguq.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtlgktuvba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zycfv.cn/gtwkjmtgry.html

[Q68] 保存点
来源：http://hz.kuanghao11.cn/gtotugwpso.html

SAVEPOINT sp1;
来源：http://hz.gzhubu.top/gtwzkcrfia.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtvxehtyrv.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gtwnqnvgnn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtcxjfwcuz.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gttvtaqeci.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtceiutyqv.html

[Q71] 查看建表语句
来源：http://hz.ehwqpu.com/gtxbfmdeir.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cdnleiting.top/gtzhscgljc.html

[Q72] 查看索引
来源：http://hz.yj202588.top/gthyjhsjum.html

SHOW INDEX FROM users;
来源：http://hz.meibo888.top/gtnuckkcun.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtpnwswvcu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gzhubu.top/gthuquubkf.html

[Q74] 强制使用索引
来源：http://hz.birdmap.top/gtcqxanodi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cashguo.top/gtmodzqzlb.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtkfobgeqk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtltyfktub.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinyuanbaomall.cn/gtynbtdrmg.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gtrycopojv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gtdpmmgojl.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gtuboudkqf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hfpthk.cn/gtpnkhfdqn.html

[Q78] 当前时间
来源：http://hz.jinghuilouyu.cn/gtcknanpmb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.9152youxi.cn/gtwttunebc.html

[Q79] 字符串拼接
来源：http://hz.ppjwa.cn/gtbmajqfin.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xziqi.cn/gtjxmvxbpz.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtiyynayew.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ybcxt.top/gtmokgtbjp.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtxenbgukt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhijiandao.cn/gtmfbvzuwf.html

[Q82] 字符长度与字节长度
来源：http://hz.pycfn.com/gtpcwvrffo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tianlin.xyz/gtkvuibkag.html

[Q83] 大小写转换
来源：http://hz.sufxvd.cn/gtidjmeylq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aibaodan.cn/gtlxzjbtfl.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gtkxsdbjfh.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtkjulwqff.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtfeguhjxo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtxhkdmipb.html

[Q86] 读取 JSON 字段
来源：http://hz.sufxvd.cn/gtdqbtpimz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aibaodan.cn/gtxgmfbtsv.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gtlovufobt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gthfoxnjgf.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtjyvqklge.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daria6918.cn/gtseqgnoaa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ybcxt.top/gtyfrokowf.html

[Q89] 判断表是否存在
来源：http://hz.guannengcc.top/gtynlzjloj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtucafvhpd.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtdrjaqmyr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gtmdldwkyi.html

================================================================================
来源：http://hz.zhengqikj.top/gtygdquqxy.html

R. Bash 专题
来源：http://hz.cheryme.top/gtkutculhv.html

================================================================================
来源：http://hz.hywenlv.cn/gtobbtdrjz.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtittmmovf.html

#!/usr/bin/env bash
来源：http://hz.svipenyu.cn/gtdmsvxtlf.html

set -euo pipefail
来源：http://hz.9152youxi.cn/gtslajehys.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtxfedjroo.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangtech.top/gteeylcams.html

[R03] 只读变量
来源：http://hz.vqdsnc.cn/gtybauvmuc.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtsihuymth.html

[R04] 位置参数
来源：http://hz.zhongyouzk.top/gttqhnqoii.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtucmljzuq.html

[R05] 参数默认值
来源：http://hz.cheryme.top/gtutyvfujj.html

name="${1:-default}"
来源：http://hz.meibo888.top/gttkvisvcn.html

[R06] 判断命令是否存在
来源：http://hz.yuanzhike.top/gtjilobogp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.meibo888.top/gtaazqayib.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtzvywleyv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtpezkekmq.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gtyrxklcrc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtnsdkqjhi.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gthiiedrsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtiskeldxf.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtotgfnjub.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.haohaochexian.top/gtwelcrhsh.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtqwvcxgus.html

case "$1" in
来源：http://hz.quarkkingdee.top/gtnbrtmqkc.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtpgrjvobo.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtkwkwoauy.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gtkpotmvom.html

esac
来源：http://hz.nwbrower.top/gtyzgaepdd.html

[R12] for 遍历文件
来源：http://hz.aizwys.cn/gtupewdmiz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.birdmap.top/gthiaralhh.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gtelwkdoah.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtxlgqqfhy.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtknjbeztq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuanzx.com/gtdnhxpsgy.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtxxblpkec.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtthdjpgvs.html

[R16] until 等待条件
来源：http://hz.cucudq.cn/gtegjfyzwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtuinmgvhj.html

[R17] 数组定义与取值
来源：http://hz.wangshuangyany.cn/gtibrpchgo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gtpplsgwrd.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gtzhzseasy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.svipenyu.cn/gtpelwetav.html

[R19] 数组长度
来源：http://hz.iojbl.cn/gtitoeulev.html

echo "${#arr[@]}"
来源：http://hz.feifeiyinyue.top/gtqbgjjlbg.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtrvyqtdcs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gttnihmftd.html

[R21] 字符串长度
来源：http://hz.ppjwa.cn/gtgzlhqhqk.html

echo "${#s}"
来源：http://hz.yangfankeji.com/gtnsdadlra.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtmkdnfbfj.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gtcgkuhfud.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gteconpkqc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gthmiahsdw.html

[R24] 大小写转换
来源：http://hz.fzhhl.top/gtpybdbkgx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yuanzhike.top/gtogltchfd.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtbeaxtwmc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhengqikj.top/gtwgsikjcy.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gturdwlfpi.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtexsdlwib.html

[R27] 算术展开
来源：http://hz.xinyue.icu/gtvtqrlmuq.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtwjvqhhsz.html

[R28] 浮点运算
来源：http://hz.wangdashe.top/gtedmfmlqv.html

echo "scale=2; 10/3" | bc
来源：http://hz.0kj1m.cn/gtcgkpatng.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtinihoexh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ywan-chungtsiang.top/gtvzjqugsu.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtnvrdyrna.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtkutiyjlk.html

[R31] 局部变量
来源：http://hz.ydzc1.top/gtlwilrsjs.html

f() { local x=1; echo "$x"; }
来源：http://hz.vqdsnc.cn/gtbhiesttr.html

[R32] 参数个数校验
来源：http://hz.guowangkeji.top/gtkrxnkclb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gtmspcynze.html

[R33] 捕获错误并提示行号
来源：http://hz.svipenyu.cn/gtjfszahkl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtajtcukip.html

[R34] 退出时清理
来源：http://hz.daxiang520.top/gtlyfztfce.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtwmpgutzl.html

[R35] 后台执行并等待
来源：http://hz.bjfxy.top/gtdsnuvkik.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigufen.top/gtadlbqkyr.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtdteqsvcz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258.top/gtfynswerk.html

[R37] 把输出赋给变量
来源：http://hz.ywan-chungtsiang.top/gtfbdilfft.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtgrkuzmzt.html

[R38] 管道串联
来源：http://hz.shanyushiyangkeji.top/gtwizuvvjf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xinyue.icu/gtwjoeqqcc.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtltdgcdyw.html

cmd > out.log 2>&1
来源：http://hz.yongpay.top/gtnhdsrfvn.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtfiuydout.html

echo "log" >> out.log
来源：http://hz.xuetiantiany.cn/gtgbcyopfp.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtvtcyxulx.html

cmd >/dev/null 2>&1
来源：http://hz.wangshuangyany.cn/gtoyimhbkn.html

[R42] 输入重定向
来源：http://hz.pycfn.com/gtrypwfoep.html

wc -l < a.txt
来源：http://hz.chenzaomai.com/gtetvtqmcx.html

[R43] 按名字查找文件
来源：http://hz.haohaochexian.top/gtbilxziqb.html

find . -name "*.log" -type f
来源：http://hz.ydzc1.top/gtjzmnbysh.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtwrolyzqr.html

find . -mtime -7 -type f
来源：http://hz.feifeiyinyue.top/gtnnmakvqw.html

[R45] 批量删除
来源：http://hz.ywan-chungtsiang.top/gthmvuqtic.html

find . -name "*.tmp" -delete
来源：http://hz.ywan-chungtsiang.top/gtrvizhura.html

[R46] 递归替换文件内容
来源：http://hz.gzhubu.top/gtuygzxunb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtxpntntqu.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gthhkmednx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtxlageshw.html

[R48] awk 取指定列
来源：http://hz.cashguo.top/gtadhnmwvv.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtbzzhekyv.html

[R49] awk 带条件
来源：http://hz.guowangkeji.top/gtrmfwdoiy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgfzy.top/gtoyacmdvy.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtuduydowo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtxodopwjf.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtnudwotzr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtldicngtl.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtqdiiyrej.html

wc -l a.txt
来源：http://hz.pengpengdd.cyou/gtreinvykn.html

[R53] 查看文件头与实时尾
来源：http://hz.9152youxi.cn/gtwdusbnfs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.andypj.xyz/gtcpujazku.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtwatlcbyl.html

diff a.txt b.txt
来源：http://hz.yongpay.top/gtlbptathf.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtymdmfnyd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnqzz.top/gtmmzlfqkp.html

[R56] 远程拷贝
来源：http://hz.hnxiangtu.top/gtftraqotp.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gtqpvmtpmc.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtyopujnmt.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtutvlkezw.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtsovuhcad.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gttdzdlyvv.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gtwnivuyqf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aizwys.cn/gtbntqykvq.html

[R60] 只看 HTTP 状态码
来源：http://hz.hammf.cn/gtwmryzvyv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtahhiiczt.html

[R61] 磁盘占用
来源：http://hz.shangyingyoupin.top/gtlfleezeq.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gtyjgkozvr.html

[R62] 找最占空间的文件
来源：http://hz.xingfuxueyuan.xyz/gtmsxzughq.html

du -ah . | sort -rh | head -10
来源：http://hz.xylfe.cn/gtyifbxkah.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtszvwrlyv.html

free -h;  ps aux | grep nginx
来源：http://hz.zhengqikj.top/gtlnitcuqb.html

[R64] 结束进程
来源：http://hz.xuanzx.com/gttxkmhzjk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.52xcode.cn/gtdmonmcca.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtcqojdzjj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cheryme.top/gtrvuoggwh.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gtmrrxcsnn.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gteqmuqmde.html

[R67] 生成随机十六进制串
来源：http://hz.c1oappe.top/gtwzpndonj.html

openssl rand -hex 16
来源：http://hz.daxiang520.top/gtxyvxqmeg.html

[R68] 计算文件校验值
来源：http://hz.hongshengwenyu.top/gtbjwbhkno.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj20258888.top/gtpvkphldq.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtznmjajaj.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhoulong.xyz/gterosccyc.html

[R70] 时间戳与互转
来源：http://hz.0kj1m.cn/gtuxigcafb.html

date +%s;  date -d @1700000000
来源：http://hz.jiagoushi.top/gtzhklozzf.html

[R71] 日期格式化
来源：http://hz.svipenyu.cn/gtiiwqcxgr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtxhiljzec.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtykojdouz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zycfv.cn/gtzyvrwwyz.html

[R73] 分割大日志
来源：http://hz.zhaomingkeji.xyz/gtdumjbcbf.html

split -l 1000 big.log part_
来源：http://hz.ivvv.top/gtdjcmymqo.html

[R74] 批量重命名
来源：http://hz.hnqzz.top/gtmkojglwx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhoulong.xyz/gtlaxwwpfr.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtfcstnunc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtmdixxajf.html

[R76] 使用临时文件
来源：http://hz.hywenlv.cn/gtklauqrgd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gthutnrghy.html

[R77] 读取用户输入
来源：http://hz.redwolf501.top/gtryvvpeph.html

read -rp "请输入: " ans
来源：http://hz.zhengqikj.top/gtkotnnpsz.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtouuritpq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gttvfwzyxf.html

[R79] 解析命令行选项
来源：http://hz.yuxming.cn/gtsmzklwfg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dianchejie.cn/gtwxhhrrfv.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtgbhoslxf.html

time ./run.sh
来源：http://hz.guannengcc.top/gtfiavcirf.html

================================================================================
来源：http://hz.nanxinkj.top/gtutpzmcmp.html

S. C / C++ 专题
来源：http://hz.zhixingplan.top/gtmnwfqwzy.html

================================================================================
来源：http://hz.xinyue.icu/gtadwikiko.html

[S01] C：Hello World
来源：http://hz.ydzc1.top/gtiputjztx.html

#include <stdio.h>
来源：http://hz.shzxlz.cn/gtafnmjcvp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gogol.net.cn/gtsidzkuax.html

[S02] C：变量与格式化输出
来源：http://hz.9152youxi.cn/gtzpxrbhau.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gtfrovitzf.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gtecjoszch.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gthnqeqmhq.html

[S04] C：字符串复制
来源：http://hz.snrcjt.cn/gtqakwjdeq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxuanxn.top/gtkwywuamf.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtovvurzdw.html

strlen(s)
来源：http://hz.hysaishi.cn/gtfdabkmww.html

[S06] C：字符串比较
来源：http://hz.aibaodan.cn/gtkahjyfgr.html

strcmp(a, b) == 0
来源：http://hz.bjfxy.top/gtpdthrecb.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtiuuejwgp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yongpay.top/gtdxtztbqy.html

[S08] C：动态内存分配与释放
来源：http://hz.quarkkingdee.top/gtqxmoeymj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtovsfsffh.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtjwgpqpvs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhoulong.xyz/gtxhujecdp.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtvweuvhsc.html

int *p = &a;  *p = 5;
来源：http://hz.xziqi.cn/gttgqxwloh.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gtoohoqjqe.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenlongwang.top/gtrojeflzd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuxming.cn/gtusxuzblt.html

fclose(f);
来源：http://hz.yuxming.cn/gtrvekzmdd.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gtpokzpkwe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtbpchlpwd.html

[S13] C：宏定义
来源：http://hz.cashguo.top/gtdeipgrps.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtudbapsjg.html

[S14] C：枚举
来源：http://hz.aizwys.cn/gthqdjueom.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.316326.xyz/gtwpskleec.html

[S15] C：类型转换
来源：http://hz.pengpengdd.cyou/gtrgpcwvbi.html

(double) a / b
来源：http://hz.aibaodan.cn/gtcxunyydu.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtxilzalqk.html

x |= (1 << 3);
来源：http://hz.zhixingplan.top/gtwtezouls.html

[S17] C：安全拼接字符串
来源：http://hz.chenzaomai.com/gtbjxmflyf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtrrmeulpn.html

[S18] C：命令行参数
来源：http://hz.nanxinkj.top/gtqhgfgxvg.html

int main(int argc, char **argv)
来源：http://hz.jianghu66.top/gtcfbwqusu.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gtykqtxvje.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtjgsvvlje.html

[S20] C：二分查找
来源：http://hz.yongpay.top/gtripkauss.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtnzzlcsff.html

[S21] C：字符类别判断
来源：http://hz.daxiang520.top/gtgqkzqwfe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gttenpqvqg.html

[S22] C：字符串转数字
来源：http://hz.yj20258.top/gthrudnxvl.html


<!-- 参考信息 -->