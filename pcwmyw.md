代发 wailian999

[Q65] 回滚事务
来源：http://hz.ywan-chungtsiang.top/gtxhqbksxx.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtukvtitmx.html

[Q66] 行锁查询
来源：http://hz.redwolf501.top/gtnjswiote.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtyyvsccvt.html

[Q67] 设置隔离级别
来源：http://hz.daxiang520.top/gtddjtgism.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guannengcc.top/gtbvpzpucl.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtckkgogtd.html

SAVEPOINT sp1;
来源：http://hz.wangdashe.top/gtlxejbxlp.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtcjonphxz.html

[Q69] 查看执行计划
来源：http://hz.yj20258.top/gtmuuzkgzs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtlatrszxl.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gtrzxmeuva.html

ANALYZE TABLE users;
来源：http://hz.sxryk.cn/gtkxeszfau.html

[Q71] 查看建表语句
来源：http://hz.jqgufenzy.top/gtmqwcqfio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cdnleiting.top/gtjdjwnxif.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gthmojnhdy.html

SHOW INDEX FROM users;
来源：http://hz.sufxvd.cn/gtwsooekts.html

[Q73] 查看表状态
来源：http://hz.jinyuanbaomall.cn/gtzbfzvbxw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zdqjudy.top/gttaqvumsv.html

[Q74] 强制使用索引
来源：http://hz.hammf.cn/gtkifrnhmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtszpcnznq.html

[Q75] 日期格式化
来源：http://hz.ydjk.org.cn/gtcoymxgkh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuanzx.com/gtfioazosd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gthhlcjgds.html

[Q76] 按天统计
来源：http://hz.shuidangran.top/gtvreqbiqu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtaylzptsq.html

[Q77] 时间加减
来源：http://hz.guowangkeji.top/gtmntzcqwc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtgqpqqlmu.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtigmbaxkp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.svipenyu.cn/gtgsazacml.html

[Q79] 字符串拼接
来源：http://hz.wangshuangyany.cn/gtunfkdaws.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnqzz.top/gtetpuqsqj.html

[Q80] 字符串截取
来源：http://hz.xinyue.icu/gtuptaygji.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtyogwgvzg.html

[Q81] 字符串替换
来源：http://hz.andypj.xyz/gtoqxlmgih.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhengqikj.top/gtobklbbor.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigufen.top/gtucqcofmq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtpfmedmyn.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gthletzyxo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtzfoqcouh.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtrdoezbrh.html

SELECT TRIM(name) FROM users;
来源：http://hz.vqdsnc.cn/gtpcmjuamb.html

[Q85] 数值取整
来源：http://hz.chenzaomai.com/gtvthheodi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydzc1.top/gtneimsrth.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangtech.top/gtsgoavjzn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yanxiufei.cn/gtpoiwulqz.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gtkzzafrtu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.c1oappe.top/gttfknbgwm.html

[Q88] 行转列（条件聚合）
来源：http://hz.jianghu66.top/gtrdpszzrb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnqzz.top/gtrpxqasco.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gttgctvyyu.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gtcgsapudz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xingfuxueyuan.xyz/gtjeftvflz.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtqwdxvbcr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtzcxvqluz.html

================================================================================
来源：http://hz.xinyue.icu/gtlhtgnjrw.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtvebwegfm.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtypnmhpxh.html

[R01] shebang 与严格模式
来源：http://hz.nwbrower.top/gtxeeeigou.html

#!/usr/bin/env bash
来源：http://hz.hnqzz.top/gtarznzadj.html

set -euo pipefail
来源：http://hz.52xcode.cn/gtfzinxfhp.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gtsivuigxs.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gtpocgcmau.html

[R03] 只读变量
来源：http://hz.zhiwuduotai.top/gtflxvnixn.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtfikrjazg.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtghwyzwmy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtbagjrfga.html

[R05] 参数默认值
来源：http://hz.snrcjt.cn/gtytmhxmew.html

name="${1:-default}"
来源：http://hz.52xcode.cn/gtcwoubxqt.html

[R06] 判断命令是否存在
来源：http://hz.ppjwa.cn/gtksocctty.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtmqwvzwoy.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gtrwerjmxw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtwhibuosy.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtyzinudsx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tian-w.cn/gtzdtisnmd.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtrwooxmrc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtzpzjkdfa.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtptzfwvij.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gttzuyrwtr.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtpblwpfrs.html

case "$1" in
来源：http://hz.cashguo.top/gtvzpoaais.html

start) echo "启动" ;;
来源：http://hz.sufxvd.cn/gthwmjsqfn.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtntsbsxwr.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtrluseiop.html

esac
来源：http://hz.ydzc1.top/gtalwvlzky.html

[R12] for 遍历文件
来源：http://hz.meibo888.top/gtjwziyunt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtriwctanr.html

[R13] for 计数循环
来源：http://hz.tanke756.top/gtkggmczjb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtrmegnzvk.html

[R14] C 风格 for
来源：http://hz.mhx1999.top/gtvmhvbzje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yueranfly.top/gtqhdihztm.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtwgjyncnl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.quarkkingdee.top/gtjqrauubw.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gttdajqacf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fengsongda.top/gtoztkpdmj.html

[R17] 数组定义与取值
来源：http://hz.dianchejie.cn/gtkhmhurdd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.redwolf501.top/gthfeacuol.html

[R18] 遍历数组
来源：http://hz.9152youxi.cn/gtyctwewlu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cashguo.top/gtqyevwrpy.html

[R19] 数组长度
来源：http://hz.zhiwuduotai.top/gtxhewmifh.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gthgkhixzs.html

[R20] 关联数组（字典）
来源：http://hz.nwbrower.top/gtomudqdml.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hysaishi.cn/gtqyrmtlqy.html

[R21] 字符串长度
来源：http://hz.ppjwa.cn/gtdwnblvke.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtchfcipvc.html

[R22] 截取子串
来源：http://hz.zhijiandao.cn/gtpqrvbqdb.html

echo "${s:0:5}"
来源：http://hz.nanxinkj.top/gtpcxdghxt.html

[R23] 字符串替换
来源：http://hz.nanxuanxn.top/gtqciaxeci.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtsghxooao.html

[R24] 大小写转换
来源：http://hz.daxiang520.top/gtoevnfhjt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dashuyun.cn/gticmybqiz.html

[R25] 去后缀 / 去前缀
来源：http://hz.cucudq.cn/gtnghgzwtj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinghuilouyu.cn/gtcylzkpqm.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gtzylnpmsw.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtcpibeffp.html

[R27] 算术展开
来源：http://hz.jinqigufen.top/gtxhopovbx.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtmxhriykf.html

[R28] 浮点运算
来源：http://hz.gaohongyu789.top/gtvislozlx.html

echo "scale=2; 10/3" | bc
来源：http://hz.vqdsnc.cn/gtivkannll.html

[R29] 定义函数
来源：http://hz.yongpay.top/gtdohqdrry.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinyuanbaomall.cn/gtyxxzqeab.html

[R30] 函数返回状态码
来源：http://hz.xuanzx.com/gtuqowisga.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.52xcode.cn/gtsbgqugro.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtnjodvxbn.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxuanxn.top/gtlzwxyvge.html

[R32] 参数个数校验
来源：http://hz.feifeiyinyue.top/gtkixpwkrw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj202588.top/gtumyvqaku.html

[R33] 捕获错误并提示行号
来源：http://hz.zhengqikj.top/gtstswvezd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtiemqpthp.html

[R34] 退出时清理
来源：http://hz.wangshuangyany.cn/gtnofbmiih.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtgaivduol.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtpoapkjsl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtmqpdqnuw.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtwtwpwpld.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtjwsvqvrx.html

[R37] 把输出赋给变量
来源：http://hz.andypj.xyz/gtnemkihsl.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtfcaonjym.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtgghgwchz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtmsisyjxw.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtvjrdglji.html

cmd > out.log 2>&1
来源：http://hz.chenlongwang.top/gtfuebsazn.html

[R40] 追加写日志
来源：http://hz.xziqi.cn/gtoruvlitm.html

echo "log" >> out.log
来源：http://hz.zdqjudy.top/gtvxtcmgmv.html

[R41] 丢弃输出
来源：http://hz.haohaochexian.top/gtvmmjwlbe.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtwdqykuhz.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gtyiollzkz.html

wc -l < a.txt
来源：http://hz.chenjidiqi.icu/gtmbdncmge.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtktoouryo.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtvhptrdty.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gttjwqvlky.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtfslnvqls.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtqrbkbath.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtvqnwefbm.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtlaitzhua.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnxiangtu.top/gtxtblpejx.html

[R47] sed 单行替换
来源：http://hz.jinqigufen.top/gtztnoraar.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtlrbxyxjn.html

[R48] awk 取指定列
来源：http://hz.yuxming.cn/gtcierudit.html

awk '{print $1, $3}' a.txt
来源：http://hz.52xcode.cn/gtnrowprva.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gthopeiuqz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydzc1.top/gtcvsweufs.html

[R50] awk 求和
来源：http://hz.dashuyun.cn/gtuxvjgidt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtvszuuwwo.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtczwjgtpe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtuxtyipfw.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtqcwsjkbc.html

wc -l a.txt
来源：http://hz.zhongyouzk.top/gtzcpsakps.html

[R53] 查看文件头与实时尾
来源：http://hz.birdmap.top/gtfiwffagy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuetiantiany.cn/gtjvyaikfa.html

[R54] 比较两个文件
来源：http://hz.hnqzz.top/gthneftirv.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtywztgscs.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gtcrehonda.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtrblcddav.html

[R56] 远程拷贝
来源：http://hz.hfpthk.cn/gtbzyabwjf.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtsyiiehzr.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gtxplutvft.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gtaaubhinh.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtpolygywn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhaomingkeji.xyz/gtuzvtpksg.html

[R59] 发 POST JSON
来源：http://hz.gogol.net.cn/gtwylgihse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hongshengwenyu.top/gtypntgvdn.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtiqgpxsmn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nwbrower.top/gtdtsavxmq.html

[R61] 磁盘占用
来源：http://hz.shuidangran.top/gtwsohynmv.html

df -h;  du -sh *
来源：http://hz.52xcode.cn/gtvgmhfehx.html

[R62] 找最占空间的文件
来源：http://hz.iojbl.cn/gtodfstgya.html

du -ah . | sort -rh | head -10
来源：http://hz.yuanzhike.top/gtvsfgelkl.html

[R63] 内存与进程
来源：http://hz.hammf.cn/gtnuoymdji.html

free -h;  ps aux | grep nginx
来源：http://hz.gotoacloud.top/gtuqazoxlo.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gtnbsuoukq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gtfxxqzrjn.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtuaaavdbz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtxeyburiz.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtvdnrebss.html

crontab -e;  crontab -l
来源：http://hz.dashuyun.cn/gtrllvtwlx.html

[R67] 生成随机十六进制串
来源：http://hz.zhijiandao.cn/gtvexdzokp.html

openssl rand -hex 16
来源：http://hz.yvedp.cn/gtknaarnzs.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gtvardynku.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ehwqpu.com/gtfsuezoyh.html

[R69] 生成随机密码
来源：http://hz.daria6918.cn/gtfitevcjr.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnqzz.top/gtlkzyatjl.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtzqjrgnpt.html

date +%s;  date -d @1700000000
来源：http://hz.shangyingyoupin.top/gtmyvdbeue.html

[R71] 日期格式化
来源：http://hz.zhixingplan.top/gtgrlvmihy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtxlyooxkd.html

[R72] 等待端口就绪
来源：http://hz.snrcjt.cn/gtcqvvkohf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtyfflvbcs.html

[R73] 分割大日志
来源：http://hz.yangfankeji.com/gttvzzzmwd.html

split -l 1000 big.log part_
来源：http://hz.jianghu66.top/gtmmbytztk.html

[R74] 批量重命名
来源：http://hz.dianchejie.cn/gtwrkfxwbv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtwyrxyzph.html

[R75] 导出环境变量
来源：http://hz.hnxiangtu.top/gtgdrhlpjv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guannengcc.top/gtgxehncan.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtlqmmrsrt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtynlulhhl.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtfpnesxmd.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtphggyrhn.html

[R78] 交互式菜单
来源：http://hz.gaohongyu789.top/gtnqusvtjx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gzhubu.top/gtbiuqafeq.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gtpvqbmfkj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.vqdsnc.cn/gtjgskchfi.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtujjmkzop.html

time ./run.sh
来源：http://hz.zhoulong.xyz/gtccztsgus.html

================================================================================
来源：http://hz.cashguo.top/gtszperhvj.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtwbfzxlmy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvifopcer.html

[S01] C：Hello World
来源：http://hz.aibaodan.cn/gtgoacszbt.html

#include <stdio.h>
来源：http://hz.hongshengwenyu.top/gtseptfeah.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtrgvwgnsd.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtpagvbvvm.html

int a = 10; printf("%d\n", a);
来源：http://hz.hywenlv.cn/gtaxixdjuy.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gtnwwuhtdl.html

int x; scanf("%d", &x);
来源：http://hz.hongshengwenyu.top/gthbejcdov.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtwpqxraia.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtwqaxvuwv.html

[S05] C：字符串长度
来源：http://hz.dashuyun.cn/gtvutxirah.html

strlen(s)
来源：http://hz.gotoacloud.top/gtphenxrgr.html

[S06] C：字符串比较
来源：http://hz.meibo888.top/gtisvdrseh.html

strcmp(a, b) == 0
来源：http://hz.hfpthk.cn/gtrhaiuedh.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtqfupcfzn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtxiplribl.html

[S08] C：动态内存分配与释放
来源：http://hz.yj202588.top/gtqggcfzce.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shuidangran.top/gtqrxnivuc.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtcooiyjam.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fzhhl.top/gtrdludgqp.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gthbwlydge.html

int *p = &a;  *p = 5;
来源：http://hz.zhongyouzk.top/gtgikyxdse.html

[S11] C：逐行读文件
来源：http://hz.guowangkeji.top/gtwldyzlsy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fzhhl.top/gtjrdhlgjg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ehwqpu.com/gtikmbsdgz.html

fclose(f);
来源：http://hz.0kj1m.cn/gtodysmesz.html

[S12] C：写文件
来源：http://hz.yonumen.top/gtofwkdtmm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtgeewogrw.html

[S13] C：宏定义
来源：http://hz.xylfe.cn/gttxxcxcft.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258.top/gtraqtfshn.html

[S14] C：枚举
来源：http://hz.xuanzx.com/gtlhxwswtc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gttijrwgpb.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gtumdsqeyi.html

(double) a / b
来源：http://hz.0kj1m.cn/gtriluilyd.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gtkxmwbzuj.html

x |= (1 << 3);
来源：http://hz.cqqwz.cn/gtwwqptxmo.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtqmtpsfjy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtmjanranm.html

[S18] C：命令行参数
来源：http://hz.daxiang520.top/gtlyjimuay.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtgzkgxcdb.html

[S19] C：快速排序
来源：http://hz.xuetiantiany.cn/gtpcosttbv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtydcpccex.html

[S20] C：二分查找
来源：http://hz.cashguo.top/gtbalbldyw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtmyhljugz.html

[S21] C：字符类别判断
来源：http://hz.guannengcc.top/gtenkgxzqz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shzxlz.cn/gtfrmcqphx.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gtchezpibm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gtxgexavqy.html

[S23] C：随机数
来源：http://hz.ydzc1.top/gttdochryi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtfnpwmdci.html

[S24] C：获取本地时间
来源：http://hz.sweek.top/gtgiyceqaf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtbbwsdldt.html

[S25] C：内存拷贝
来源：http://hz.hfpthk.cn/gtbepwbqqa.html

memcpy(dst, src, n);
来源：http://hz.ydzc1.top/gthvryzyzd.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtetmgkati.html

memset(a, 0, sizeof a);
来源：http://hz.gogol.net.cn/gtvjpqjefh.html

[S27] C：定义常量
来源：http://hz.yongpay.top/gtyonoyjsu.html

const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtblojbmvk.html

[S28] C：静态变量
来源：http://hz.ivvv.top/gttuodfcqo.html

static int counter = 0;
来源：http://hz.ybcxt.top/gtwvsvadql.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gtnasxjtdm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ehwqpu.com/gtjmyyjbql.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtrzmgswrm.html

#ifndef X_H
来源：http://hz.dashuyun.cn/gtqbjkffzh.html

#define X_H
来源：http://hz.ybcxt.top/gtgwosokya.html

#endif
来源：http://hz.wangshuangyany.cn/gtepciifkt.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtrsuyfesy.html

#include <iostream>
来源：http://hz.sufxvd.cn/gtkhsakiiz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.birdmap.top/gtqgkbeofz.html

[S32] C++：字符串
来源：http://hz.chenzaomai.com/gtqbtdggzv.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gtxlryyvvy.html

[S33] C++：vector 增删
来源：http://hz.havefunace.top/gthrkjszyb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtaypnqoky.html

[S34] C++：遍历 vector
来源：http://hz.guowangkeji.top/gtpjstqxst.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.iojbl.cn/gtbpbzlvlh.html


<!-- 参考信息 -->