代发 wailian999

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtbscgsxhs.html

ROLLBACK;
来源：http://hz.sufxvd.cn/gtnteaevig.html

[Q66] 行锁查询
来源：http://hz.dianchejie.cn/gtaqkodwqi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gotoacloud.top/gtdwylaiew.html

[Q67] 设置隔离级别
来源：http://hz.vqdsnc.cn/gtkhdmvjjl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gthcmmpqba.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtrsrdalbd.html

SAVEPOINT sp1;
来源：http://hz.zhijiandao.cn/gtrorafenn.html

ROLLBACK TO sp1;
来源：http://hz.shzxlz.cn/gtuxdkozqg.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gttowoiwej.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.vqdsnc.cn/gtcjcvqdcq.html

[Q70] 更新统计信息
来源：http://hz.nwbrower.top/gtqqmibtzg.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtnmlrvgbn.html

[Q71] 查看建表语句
来源：http://hz.vqdsnc.cn/gtukxzulxx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtqlmcmlnk.html

[Q72] 查看索引
来源：http://hz.wangdashe.top/gtkzblmxiu.html

SHOW INDEX FROM users;
来源：http://hz.c1oappe.top/gtjrxmeggi.html

[Q73] 查看表状态
来源：http://hz.jinghuilouyu.cn/gtigqhoyml.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtprbvwpit.html

[Q74] 强制使用索引
来源：http://hz.ydjk.org.cn/gtxmlyryzi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258888.top/gtiignoqoz.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gteqpbbymt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnqzz.top/gtcvjkvotz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtosihfjzz.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtlmcrieav.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cashguo.top/gtxtnwkkoi.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtkxgmwvev.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhoulong.xyz/gtkbuiryjf.html

[Q78] 当前时间
来源：http://hz.ppjwa.cn/gtfsooeail.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tianlin.xyz/gtlikhoooc.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtdvzxyrec.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dashuyun.cn/gtuzntbsyh.html

[Q80] 字符串截取
来源：http://hz.hnqzz.top/gtxrxltplg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuetiantiany.cn/gtxlqcjnfv.html

[Q81] 字符串替换
来源：http://hz.52xcode.cn/gtvuudczil.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtjloooqlc.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gtawotcpkn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhengqikj.top/gttfulhvsh.html

[Q83] 大小写转换
来源：http://hz.sufxvd.cn/gtrzxmfkyl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgufenzy.top/gtygdosjpk.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtjbmnlovd.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtggjqrhha.html

[Q85] 数值取整
来源：http://hz.redwolf501.top/gtjuzzvrrk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hammf.cn/gttzydtpag.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gtsylhdiho.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinyuanbaomall.cn/gtmwbhkgtk.html

[Q87] JSON 字段做条件
来源：http://hz.aibaodan.cn/gtthqfhzvb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtkmpkkpwk.html

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtwyyylqeg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtactlitjp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtbxajieic.html

[Q89] 判断表是否存在
来源：http://hz.yangfankeji.com/gtwqnbidyi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangtech.top/gticgjndgw.html

[Q90] 生成序号列
来源：http://hz.sxryk.cn/gttchhshmi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yvedp.cn/gtjcrpinuq.html

================================================================================
来源：http://hz.tian-w.cn/gtoytckaky.html

R. Bash 专题
来源：http://hz.feifeiyinyue.top/gthscowrzl.html

================================================================================
来源：http://hz.cdnleiting.top/gtofbijxsh.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gttphnxlkc.html

#!/usr/bin/env bash
来源：http://hz.cashguo.top/gtakuoajgm.html

set -euo pipefail
来源：http://hz.9152youxi.cn/gtijckrarj.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gthcuvjbis.html

name="Tom"; echo "$name"
来源：http://hz.yueranfly.top/gtrnbsfeed.html

[R03] 只读变量
来源：http://hz.gotoacloud.top/gthpydpqrn.html

readonly PI=3.14
来源：http://hz.fengsongda.top/gtqytcbjid.html

[R04] 位置参数
来源：http://hz.yuanzhike.top/gtjofhappu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxinkj.top/gtjqldbxhg.html

[R05] 参数默认值
来源：http://hz.nwbrower.top/gtmtztubjc.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtxlasdsdd.html

[R06] 判断命令是否存在
来源：http://hz.cashguo.top/gtffvllngk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jianghu66.top/gtdteuzwdm.html

[R07] if 判断文件
来源：http://hz.chenzaomai.com/gtbnmxurpi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tanke756.top/gtcbsouycm.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gtbkwibwol.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtwxeptbig.html

[R09] 字符串比较
来源：http://hz.yj20258888.top/gtavtxcqyy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gtaovkalyc.html

[R10] 正则匹配
来源：http://hz.hongshengwenyu.top/gtopbwvbox.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhijiandao.cn/gtlcvfffzz.html

[R11] case 多分支
来源：http://hz.yuxming.cn/gtwshhrtws.html

case "$1" in
来源：http://hz.aizwys.cn/gtnmqjscwa.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtcglhvkuo.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtjtkqrjvz.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtboyfsurx.html

esac
来源：http://hz.dashuyun.cn/gtkjfprzwv.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gthviyrwmn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtihjkyffh.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gthkwewgir.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnxiangtu.top/gthuhwcnrr.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gtosawlsvc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.smart0.xyz/gtetqquzvc.html

[R15] while 逐行读文件
来源：http://hz.yvedp.cn/gtdonufgpi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.quarkkingdee.top/gtqtbzxrka.html

[R16] until 等待条件
来源：http://hz.tianlin.xyz/gtarbqctep.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtqlibzshb.html

[R17] 数组定义与取值
来源：http://hz.jinghuilouyu.cn/gtamwyhphi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtoykqkiyo.html

[R18] 遍历数组
来源：http://hz.cucudq.cn/gtnnvkytnp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.birdmap.top/gtbkqryzfm.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtlzlftane.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtmqttljns.html

[R20] 关联数组（字典）
来源：http://hz.yonumen.top/gtumprhiaw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cucudq.cn/gtuyojwwcj.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtwupibcuj.html

echo "${#s}"
来源：http://hz.cqqwz.cn/gtehcfdezd.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtkbziaixj.html

echo "${s:0:5}"
来源：http://hz.ivvv.top/gtxncqsxkq.html

[R23] 字符串替换
来源：http://hz.yuxming.cn/gtzmlmlwur.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jlsjyb.cn/gtzqywiisg.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gteheosvil.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangdashe.top/gtqxffoxta.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtsjhjbspm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.316326.xyz/gtzntgipam.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtcuuksalz.html

now=$(date +%F); echo "$now"
来源：http://hz.cheryme.top/gtxbukvfra.html

[R27] 算术展开
来源：http://hz.yonumen.top/gtuqglyfpw.html

echo $((1 + 2 * 3))
来源：http://hz.bjfxy.top/gtjsdikimp.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gttsmjxnuq.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gthizicyjp.html

[R29] 定义函数
来源：http://hz.tian-w.cn/gthlpvflga.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydzc1.top/gtywkqjdsm.html

[R30] 函数返回状态码
来源：http://hz.sufxvd.cn/gtbdonkwux.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtszekoiub.html

[R31] 局部变量
来源：http://hz.zhaomingkeji.xyz/gtjnzdmwyd.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtnntymyzr.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtsvultlik.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.52xcode.cn/gtwbqjcpyg.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtpxsbxncg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cucudq.cn/gtbevumnxt.html

[R34] 退出时清理
来源：http://hz.jqgfzy.top/gttpaznprl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtcmbqqkqv.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtigiyvjrv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dashuyun.cn/gtwimhchik.html

[R36] 并发执行多个任务
来源：http://hz.shzxlz.cn/gtafftyoyy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gogol.net.cn/gtrwpasoyq.html

[R37] 把输出赋给变量
来源：http://hz.jinqigfzy.top/gtwfjroswq.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gtkvhnkahy.html

[R38] 管道串联
来源：http://hz.xinyue.icu/gtpueqvwir.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gthdpenmuv.html

[R39] 重定向标准输出与错误
来源：http://hz.daxiang520.top/gthiapicec.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gtzwppichf.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtywhnoqhn.html

echo "log" >> out.log
来源：http://hz.jianghu66.top/gtpmqlvxfz.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtyjsqvsom.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangtech.top/gthgnufpoo.html

[R42] 输入重定向
来源：http://hz.zdqjudy.top/gtnbhktohy.html

wc -l < a.txt
来源：http://hz.chenjidiqi.icu/gtmqtdaasq.html

[R43] 按名字查找文件
来源：http://hz.guowangkeji.top/gttyqwojpq.html

find . -name "*.log" -type f
来源：http://hz.bjfxy.top/gtddlqbqvm.html

[R44] 按修改时间查找
来源：http://hz.feifeiyinyue.top/gtvjtsmycj.html

find . -mtime -7 -type f
来源：http://hz.yangfankeji.com/gtaztqshjw.html

[R45] 批量删除
来源：http://hz.cdnleiting.top/gtvfolfqzx.html

find . -name "*.tmp" -delete
来源：http://hz.yongpay.top/gtwupbothv.html

[R46] 递归替换文件内容
来源：http://hz.jyoumei.cn/gtbnbbgopd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jyoumei.cn/gtnpcjpwdg.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gtjcjpsqpm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.smart0.xyz/gtgsjbpikg.html

[R48] awk 取指定列
来源：http://hz.zhoulong.xyz/gtbpotmlin.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtrwfhesqv.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtehfbnymw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangkeji.top/gtdvqyyihp.html

[R50] awk 求和
来源：http://hz.chenjidiqi.icu/gtjvnoosmr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtkxzsnzia.html

[R51] 排序去重取前几
来源：http://hz.cqqwz.cn/gtudtmqufa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxinkj.top/gtbmhwpsdq.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtbcakvmht.html

wc -l a.txt
来源：http://hz.tanke756.top/gtwtkmwyty.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtvtxrhdve.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuetiantiany.cn/gtwuyxtgol.html

[R54] 比较两个文件
来源：http://hz.cdnleiting.top/gtylmwnwjk.html

diff a.txt b.txt
来源：http://hz.daria6918.cn/gtqsvsrlst.html

[R55] 压缩与解压
来源：http://hz.yuanzhike.top/gtqwjhzmfv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.316326.xyz/gttslondyf.html

[R56] 远程拷贝
来源：http://hz.zhijiandao.cn/gtqghevgvy.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtiulknfhu.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtxetnmcfq.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gtifaztxep.html

[R58] 下载文件
来源：http://hz.tianlin.xyz/gtpscrubjt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtyparikxn.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gtlalpyoat.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj202588.top/gtxdokoqlc.html

[R60] 只看 HTTP 状态码
来源：http://hz.cashguo.top/gtgedtwxul.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangshuangyany.cn/gtynqbftal.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtitxdyxts.html

df -h;  du -sh *
来源：http://hz.sysykeji.top/gtizmeybcn.html

[R62] 找最占空间的文件
来源：http://hz.zhiwuduotai.top/gtrfkbkthi.html

du -ah . | sort -rh | head -10
来源：http://hz.bjfxy.top/gtuftolfsj.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gtlmxasgee.html

free -h;  ps aux | grep nginx
来源：http://hz.cashguo.top/gtglrxrept.html

[R64] 结束进程
来源：http://hz.mhx1999.top/gtwjnyqbbr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.feifeiyinyue.top/gtwjyuartb.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtiefysysy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtxfcbrlfb.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gtefjhfsve.html

crontab -e;  crontab -l
来源：http://hz.dianchejie.cn/gtklnuhfev.html

[R67] 生成随机十六进制串
来源：http://hz.sysykeji.top/gtzgajcujx.html

openssl rand -hex 16
来源：http://hz.zhoulong.xyz/gtoqjiyyrn.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtzhnbyvxa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtnglvpdei.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gtythbiykt.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtnywqqxfa.html

[R70] 时间戳与互转
来源：http://hz.zhixingplan.top/gthbfyyzft.html

date +%s;  date -d @1700000000
来源：http://hz.jyoumei.cn/gtgeiticui.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtrpnhlwyg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhijiandao.cn/gtkwajsiti.html

[R72] 等待端口就绪
来源：http://hz.yuanzhike.top/gtwjtppeag.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gthwfrzoys.html

[R73] 分割大日志
来源：http://hz.zhijiandao.cn/gtrwkfrisa.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtaxzkrcij.html

[R74] 批量重命名
来源：http://hz.aizwys.cn/gtlwkqhnwh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinyuanbaomall.cn/gtzbcgxlpg.html

[R75] 导出环境变量
来源：http://hz.yj20258888.top/gttmfvpsdx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuanzx.com/gtjqyeoocv.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtbxmbgxub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtymfvhzli.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtljtgpuwq.html

read -rp "请输入: " ans
来源：http://hz.xylfe.cn/gtsfnpgqot.html

[R78] 交互式菜单
来源：http://hz.fzhhl.top/gtgumjniaj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.bjfxy.top/gtzlwerklh.html

[R79] 解析命令行选项
来源：http://hz.hnqzz.top/gtxwrtzsxn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtlpghgkos.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtvgubbupd.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gtkuxbwetv.html

================================================================================
来源：http://hz.yj20258.top/gttgikbvlb.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gteucxqirf.html

================================================================================
来源：http://hz.jianghu66.top/gtgladywxc.html

[S01] C：Hello World
来源：http://hz.guowangkeji.top/gtzhbludpb.html

#include <stdio.h>
来源：http://hz.meibo888.top/gtqkgaqabk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yueranfly.top/gtqapinqwv.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtpauowdik.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gtsxiucsjf.html

[S03] C：读入整数
来源：http://hz.daxiang520.top/gtiiknccwb.html

int x; scanf("%d", &x);
来源：http://hz.zdqjudy.top/gthbljdnik.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gtswurhokd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtmcaadwvw.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtzbhentby.html

strlen(s)
来源：http://hz.wangdashe.top/gthnzznfxw.html

[S06] C：字符串比较
来源：http://hz.zhongyouzk.top/gtpwhcolyi.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtrrxiaxbe.html

[S07] C：数组遍历求和
来源：http://hz.hongshengwenyu.top/gtfrveqevp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtfozmwhfz.html

[S08] C：动态内存分配与释放
来源：http://hz.hnqzz.top/gthqlfoptv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtklqzrtbh.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gtjqtqzikg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtpbusfzqe.html

[S10] C：指针与解引用
来源：http://hz.ydzc1.top/gtmnolhbhp.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtyanpmbod.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gtxatheykc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gteeqdcbjb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guowangkeji.top/gtzyvhpbqf.html

fclose(f);
来源：http://hz.cheryme.top/gtbbfcgbej.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtqpiwtutc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gtyznodocm.html

[S13] C：宏定义
来源：http://hz.xingfuxueyuan.xyz/gtzorizyny.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtsziflzgd.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtfiqahuwv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtletzrpee.html

[S15] C：类型转换
来源：http://hz.smart0.xyz/gtwytntljr.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtbyqriyfb.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtgeguainm.html

x |= (1 << 3);
来源：http://hz.nwbrower.top/gtkqrfmbhh.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gtykmvgaee.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.mhx1999.top/gtqsxuqegb.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtjiupanbu.html

int main(int argc, char **argv)
来源：http://hz.ywan-chungtsiang.top/gttnytvbzo.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtcmkwbsyf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gttdoccanx.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gttfswzhzl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtujatouex.html

[S21] C：字符类别判断
来源：http://hz.ydjk.org.cn/gtibappoer.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hysaishi.cn/gtvgfcncku.html

[S22] C：字符串转数字
来源：http://hz.yuanzhike.top/gtumajqydo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtkaksmcms.html

[S23] C：随机数
来源：http://hz.chenzaomai.com/gtuqzkxrvv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ehwqpu.com/gtwrdzlctr.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtbkydtmdt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yangfankeji.com/gtbxcnogqp.html

[S25] C：内存拷贝
来源：http://hz.andypj.xyz/gtkblavcoo.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtmdufqjsy.html

[S26] C：内存清零
来源：http://hz.gaohongyu789.top/gtwfleibkf.html

memset(a, 0, sizeof a);
来源：http://hz.pycfn.com/gtqcwwgcmr.html

[S27] C：定义常量
来源：http://hz.shanyushiyangtech.top/gtdgppkvvj.html

const double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtaljpahux.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gtnlurojzb.html

static int counter = 0;
来源：http://hz.hysaishi.cn/gtlqvvkyeo.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gtceihlzdm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtsowrlwjn.html

[S30] C：头文件保护
来源：http://hz.ehwqpu.com/gteqvfpopi.html

#ifndef X_H
来源：http://hz.chenlongwang.top/gttpfxfizb.html

#define X_H
来源：http://hz.jinyuanbaomall.cn/gtqjfroqke.html

#endif
来源：http://hz.ydjk.org.cn/gtqbvkshsw.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtnnaoyuah.html

#include <iostream>
来源：http://hz.iojbl.cn/gtjplpeizd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fzhhl.top/gtssgvwozr.html

[S32] C++：字符串
来源：http://hz.shangyingyoupin.top/gtbtukfpqu.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtgoodpgvn.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gtewkiuixv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtpewezmog.html

[S34] C++：遍历 vector
来源：http://hz.ehwqpu.com/gtopxzzkcr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guowangkeji.top/gtjmftlxno.html


<!-- 参考信息 -->